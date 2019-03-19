# Programa-Monitora-Modulo-Basico-Mamiferos
Taxas anuais de avistamento em transecções lineares

Função para calcular taxas de avistamento a partir dos dados de transecções lineares do **Programa Monitora-ICMBio**.

A função gera dataframes e gráficos (Figura 1) com taxas de avistamento (encontros a cada 10 km percorridos) para cada dia de contagem nas trilhas, e taxas anuais médias e SD para cada unidade de Conservação. O SD é estimado combinando os dados das diferentes contagens num mesmo ano (geralmente 15 contagens, equivalente a 150 km percorridos por ano).

A função utiliza o csv da planilha **"mastoaves"** do Programa Monitora-ICMBio. é preciso especificar os dados, a UC e a espécie de interesse.


![Rplot01](https://user-images.githubusercontent.com/39089964/54637985-b974bb00-4a68-11e9-9dc5-a223556e5fda.jpeg)

Figura 1. Taxas de avistamento de *Dasyprocta fuliginosa* na FLONA do JAMARI, 2014-2018. O envelope sombreado correponde ao SD.

Contribuições são bem vindas!
