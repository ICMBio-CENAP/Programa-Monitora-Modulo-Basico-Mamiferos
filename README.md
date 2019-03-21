# Programa-Monitora-Modulo-Basico-Mamiferos
Taxas anuais de avistamento em transecções lineares.

Função para calcular taxas de avistamento a partir dos dados de transecções lineares do **Programa Monitora-ICMBio**.

A função gera dataframes e gráficos (Figura 1) com taxas de avistamento (encontros a cada 10 km percorridos) para cada transecção, bem como médias anuais e SD das taxas de avistamento. Médias e SD são estimados a partir do conjunto de transecções realizadas em cada ano (geralmente 15 transecções por ano, equivalente a 150 km percorridos).

A função utiliza o csv da planilha **"mastoaves"** do Programa Monitora-ICMBio. Para chamar a função é preciso especificar o conjunto de dados, a UC e a espécie de interesse.


![Rplot](https://user-images.githubusercontent.com/39089964/54756509-24d49f00-4bc7-11e9-866e-6499e10a4731.jpeg)

Figura 1. Taxas de avistamento de *Dasyprocta fuliginosa* na FLONA do JAMARI, 2014-2018. O envelope sombreado correponde ao SD.


### Instruções para execução do script

1 - Instale os pacotes **openair** e **ggplot2** do R

```r
install.packages("openair")
install.packages("ggplot2")
```

Com isso o script pode ser executado normalmente


### Instruções para rodar a função

Depois de ler a função **monitora1**, basta chamar a função como no exemplo

```r
monitora1(dados, "Flona do Jamari", "Dasyprocta cf. fuliginosa") # roda a função para a espécie *D. fuliginosa* somente para Flona do Jamari
monitora1(dados, z="Dasyprocta cf. fuliginosa") roda a função para a espécie *D. fuliginosa* incluindo todas as UCs onde a espécie ocorreu

```

Contribuições são bem vindas! Também agradecemos se alguém nos informar sobre eventuais erros.
