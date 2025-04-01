# Detecção de Anomalias
![Gráfico 1](https://github.com/user-attachments/assets/7027c856-7de8-406f-9bd7-ad3a22fba493)

# Descrição
O objetivo deste estudo é aplicar técnicas de detecção de anomalias, especificamente o Isolation Forest e o DBSCAN, a um conjunto de dados de contas financeiras. O propósito é identificar contas de transações que se desviam significativamente do comportamento típico, o que pode indicar atividades fraudulentas ou incomuns.

# Etapas
Primeiramente, foram feitos os tratamentos e análises exploratórias dos dados para avaliações e saber que tipo de informações iniciais podemos obter. De acordo com as análises exploratórias, os dados apresentavam muitos outliers e alta assimetria, o que pode prejudicar a detecção de anomalias, além de que os dados numéricos estavam em escalas diferentes, tornando necessária a normalização para padronizá-los.

Essa combinação de processos reduziu bastante o número de outliers e a assimetria das distribuições, aproximando-as de uma gaussiana (normal).

Na etapa seguinte, realizamos a redução de dimensionalidade usando PCA com o objetivo de encontrar o menor número de componentes principais possível, preservando o máximo de informação (variância) dos dados. Como resultado, reduzimos ruídos e diminuímos os custos computacionais.

Após reduzirmos a dimensionalidade da base de dados com o método PCA, entramos nos modelos de detecção de anomalias, aplicando o algoritmo DBSCAN e Isolation Forest, dois métodos poderosos para clusterização e detecção de anomalias.  Com base nessas etapas, encontramos o cluster anômalo que apresentam um padrão de comportamento muito diferente dos demais clusters. Algumas características foram:

* Gastam muito mais (especialmente compras pontuais).

* Fazem menos compras, mas de alto valor.

* Usam mais adiantamentos de dinheiro.

* Têm um limite de crédito maior.

* Pagam valores mais altos e mais frequentemente a fatura completa.

* São clientes há menos tempo.
