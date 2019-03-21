# Programa-Monitora-Modulo-Basico-Mamiferos
Taxas anuais de avistamento em transecções lineares.

Função para calcular taxas de avistamento a partir dos dados de transecções lineares do **Programa Monitora-ICMBio**.

A função gera dataframes e gráficos (Figura 1) com taxas de avistamento (encontros a cada 10 km percorridos) para cada transecção, bem como médias anuais e SD das taxas de avistamento. Médias e SD são estimados a partir do conjunto de transecções realizadas em cada ano (geralmente 15 transecções por ano, equivalente a 150 km percorridos).

A função utiliza o csv da planilha **"mastoaves"** do Programa Monitora-ICMBio. Para chamar a função é preciso especificar o conjunto de dados, a UC e a espécie de interesse.


![Rplot](https://user-images.githubusercontent.com/39089964/54756509-24d49f00-4bc7-11e9-866e-6499e10a4731.jpeg)

Figura 1. Taxas de avistamento de *Dasyprocta fuliginosa* na FLONA do JAMARI, 2014-2018. O envelope sombreado correponde ao SD.


### Pré-requisitos

Instale os pacotes **openair** e **ggplot2** do R

```r
install.packages("openair")
install.packages("ggplot2")
```

Com isso o script pode ser executado normalmente


### Instruções para rodar a função

Depois de copiar e rodar a função **monitora1** no script, basta aplicar aos dados da UC e espécie de interesse conforme o exemplo:

```r
monitora1(dados, "Flona do Jamari", "Dasyprocta cf. fuliginosa") # roda a função para *D. fuliginosa* somente para Flona do Jamari
monitora1(dados, z="Dasyprocta cf. fuliginosa") # roda a função para *D. fuliginosa* incluindo todas as UCs onde a espécie ocorreu
monitora1(dados, y=c("Resex Cazumbá-iracema", "Resex Tapajós-Arapiuns"), z="Dasyprocta cf. fuliginosa") # roda a função para *D. fuliginosa* incluindo duas Resex simultaneamente
```

A função gera o gráfico automaticamente. Para visualizar os dataframes com as taxas de avistamento:
```r
taxas.por.contagem # exibe as taxas de avistamento por transecção individual
taxas.medias.anuais # exibe as taxas médias de avistamento por ano e SD 
```

Observação: Algumas UCs possuem dados incompletos para alguns anos (por exemplo, apenas uma trilha do Monitora implantada em 2014), nesses casos, é recomendável excluir esses anos da planilha ANTES de rodar a função.

Contribuições são bem vindas! Também agradecemos se alguém nos informar sobre eventuais erros.
