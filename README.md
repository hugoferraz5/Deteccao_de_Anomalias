# Detecção de Anomalias
![Gráfico 1](https://github.com/user-attachments/assets/7027c856-7de8-406f-9bd7-ad3a22fba493)

## Descrição
O objetivo deste estudo é aplicar técnicas de detecção de anomalias, especificamente o Isolation Forest e o DBSCAN, a um conjunto de dados de contas financeiras. O propósito é identificar contas de transações que se desviam significativamente do comportamento típico, o que pode indicar atividades fraudulentas ou incomuns.

Projeto Completo: [Detecção de Anomalias](https://github.com/hugoferraz5/Deteccao_de_Anomalias/blob/main/deteccao_anomalias.ipynb)

## Etapas
Primeiramente, realizamos o tratamento e a análise exploratória dos dados para avaliar suas características e obter informações iniciais. Nessa etapa, identificamos a presença de muitos outliers e alta assimetria, fatores que podem influenciar a modelagem dos dados. Além disso, os dados numéricos estavam em escalas diferentes, tornando necessária a normalização para padronizá-los.

Após a normalização, houve uma redução na influência dos outliers e na assimetria das distribuições, aproximando-as de uma distribuição normal.
Em seguida, aplicamos a redução de dimensionalidade utilizando PCA, com o objetivo de encontrar a menor quantidade de componentes principais possível, preservando a maior parte da variância dos dados. Esse processo ajudou a reduzir ruídos e diminuir os custos computacionais.

Com a base transformada, utilizamos modelos de detecção de anomalias, aplicando os algoritmos DBSCAN e Isolation Forest. O DBSCAN, além de realizar clusterização, identifica pontos classificados como ruído, que podem representar anomalias. Já o Isolation Forest é um modelo específico para a detecção de anomalias, baseado no isolamento dos pontos de dados.
A partir dessas análises, identificamos padrões anômalos nos dados, representados por clusters ou pontos isolados com comportamento significativamente diferente dos demais.
Algumas características foram:

* Gastam muito mais (especialmente compras pontuais).

* Fazem menos compras, mas de alto valor.

* Usam mais adiantamentos de dinheiro.

* Têm um limite de crédito maior.

* Pagam valores mais altos e mais frequentemente a fatura completa.

* São clientes há menos tempo.
