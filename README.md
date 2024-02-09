# Sistema de Recomendação de Músicas com Apache Spark e Spotify
Este projeto implementa um sistema de recomendação de músicas utilizando a linguagem de programação Python, com foco em processamento distribuído usando o Apache Spark. A integração com a API do Spotify também é realizada para enriquecer as informações sobre as músicas recomendadas.

## Etapas do Projeto
### 1. Configuração Inicial
O código inicia uma sessão Spark para processamento distribuído e importa bibliotecas necessárias, incluindo componentes do PySpark para processamento em larga escala e a biblioteca Spotipy para interação com a API do Spotify.

### 2. Leitura e Pré-processamento de Dados
Os dados das músicas são lidos a partir de um arquivo CSV hospedado no GitHub. O conjunto de dados passa por verificações para identificar valores nulos, e uma filtragem é aplicada para considerar apenas músicas a partir do ano 2000.

### 3. Análise e Visualização de Dados
A biblioteca Plotly é utilizada para criar visualizações interativas que ajudam na análise de tendências, como a variação do "loudness" ao longo dos anos.

### 4. Redução de Dimensionalidade com PCA
A Análise de Componentes Principais (PCA) é aplicada para redução de dimensionalidade nas características das músicas, facilitando a análise e clusterização.

### 5. Clusterização com K-Means
O algoritmo K-Means é empregado para agrupar as músicas em clusters, identificando padrões e similaridades entre elas.

### 6. Recomendação de Músicas Semelhantes
Com base nos clusters formados, o sistema recomenda músicas semelhantes a uma entrada específica, utilizando distâncias euclidianas entre os componentes do PCA.

### 7. Visualização de Capas de Álbuns Recomendados
As capas dos álbuns das músicas recomendadas são exibidas para uma experiência visual aprimorada.
