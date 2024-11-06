## ALUNO: PEDRO VICTOR SOARES FERREIRA

https://youtu.be/6ANIfc9NveQ

# Análise de Mobilidade no Entorno da UFRN - Natal/RN

Este projeto realiza uma análise de mobilidade no entorno da Universidade Federal do Rio Grande do Norte (UFRN), em Natal, RN, com foco em identificar locais estratégicos para a instalação de estações de compartilhamento de bicicletas (dock-stations). Para isso, usamos métricas de centralidade e outras análises de rede aplicadas à malha viária de bairros específicos: Potilândia, UFRN e Mirassol.

## Objetivos

- Avaliar a mobilidade nos bairros ao redor da UFRN.
- Identificar locais ideais para a colocação de dock-stations de bicicletas, considerando métricas de centralidade.
- Visualizar a rede com destaque para os nós estratégicos de acordo com as análises realizadas.

## Metodologia

1. **Coleta da Rede Viária**:
   - Utilizamos a biblioteca **OSMnx** para baixar a rede de ruas nos bairros selecionados ao redor da UFRN.
   - A rede foi obtida em formato de grafo, com as ruas como arestas e as intersecções como nós.

2. **Métricas de Centralidade**:
   - Calculamos as seguintes métricas de centralidade utilizando a biblioteca **NetworkX**:
     - **Degree Centrality**: Mede o número de conexões diretas de cada nó.
     - **Closeness Centrality**: Mede a distância média entre um nó e todos os outros, identificando nós bem conectados.
     - **Betweenness Centrality**: Mede a frequência com que um nó aparece nos caminhos mais curtos entre outros nós, ajudando a identificar pontos críticos na rede.
     - **Eigenvector Centrality**: Mede a importância de um nó considerando a conectividade dos seus vizinhos.

3. **Identificação de Locais para Dock-Stations**:
   - Selecionamos os 10 nós com maior **betweenness centrality** como sugestões para a colocação de estações de bicicletas. Esses pontos têm uma posição estratégica na rede, por estarem localizados nos caminhos mais curtos entre outros nós.

4. **Análise de Distribuição dos Graus**:
   - Realizamos uma análise de distribuição dos graus dos nós na rede, usando a função de densidade de probabilidade (PDF) e a função de distribuição acumulada (CDF), o que ajuda a entender a conectividade média da rede.

5. **Análise Multivariada das Métricas de Centralidade**:
   - Criamos visualizações para examinar as relações entre as diferentes métricas de centralidade (Degree, Closeness, Betweenness e Eigenvector).

6. **Core/Shell da Rede**:
   - Identificamos o core máximo da rede, isto é, os nós com maior conectividade mínima, para entender o núcleo estrutural da malha viária.

## Resultados

- Identificamos locais ideais para as dock-stations de bicicletas, destacando os nós com alta **betweenness centrality**.
- A análise das métricas de centralidade indicou pontos chave para a mobilidade no entorno da UFRN.
- A visualização final da rede destaca os nós com maior importância na centralidade de autovetor (**Eigenvector Centrality**), com os nós estratégicos (top nodes) exibidos em vermelho e tamanho maior.

## Visualizações

- **Mapa da Rede com Eigenvector Centrality**: Visualização da rede viária, destacando os nós com alta centralidade de autovetor e os locais sugeridos para dock-stations em vermelho.
- **Distribuição dos Graus (PDF e CDF)**: Visualizações que mostram a distribuição das conexões dos nós na rede.
