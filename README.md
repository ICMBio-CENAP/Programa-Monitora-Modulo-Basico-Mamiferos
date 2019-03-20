# Programa-Monitora-Modulo-Basico-Mamiferos
Taxas anuais de avistamento em transecções lineares

Função para calcular taxas de avistamento a partir dos dados de transecções lineares do **Programa Monitora-ICMBio**.

A função gera dataframes e gráficos (Figura 1) com taxas de avistamento (encontros a cada 10 km percorridos) para cada transecção, bem como médias anuais e SD das taxas de avistamento. Médias e SD são estimados a partir das transecções realizadas em determinado ano (geralmente 15 transecções por ano, equivalente a 150 km percorridos).

A função utiliza o csv da planilha **"mastoaves"** do Programa Monitora-ICMBio. Para chamar a função é preciso especificar o conjunto de dados, a UC e a espécie de interesse.


![Rplot01](https://user-images.githubusercontent.com/39089964/54637985-b974bb00-4a68-11e9-9dc5-a223556e5fda.jpeg)

Figura 1. Taxas de avistamento de *Dasyprocta fuliginosa* na FLONA do JAMARI, 2014-2018. O envelope sombreado correponde ao SD.

Contribuições são bem vindas! Também agradecemos se alguém nos informar sobre eventuais erros.
