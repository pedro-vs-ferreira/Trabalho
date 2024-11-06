# Análise de Rede da Cidade de Natal-RN

Este projeto implementa uma análise de rede para a cidade de Natal-RN usando as bibliotecas `osmnx` e `networkx`. O objetivo é explorar métricas de rede como comprimento médio do caminho mais curto, diâmetro da rede, coeficiente de aglomeração, entre outras, com o objetivo de entender as características de conectividade na região. Além disso, o projeto inclui a busca do caminho mais curto entre dois pontos específicos na cidade: **do Shopping Cidade Jardim até a Escola de Ciências e Tecnologia (ECT)** da UFRN.

## Estrutura do Projeto

- **Código Python**: Um script Python que cria e analisa um grafo da rede de Natal-RN.
- **Métricas Calculadas**:
  - **Número de Componentes Conectados**
  - **Tamanho do Maior Componente Conectado**
  - **Comprimento Médio do Caminho Mais Curto**
  - **Diâmetro da Rede**
  - **Coeficiente de Aglomeração**
  - **Comprimento do Caminho Mais Curto entre dois pontos**
  - **Ciclos na Rede**

## Pré-requisitos

- Python 3.7 ou superior
- Bibliotecas:
  - `osmnx`
  - `networkx`
  - `matplotlib`

## Métricas de Rede
- O código calcula as seguintes métricas de rede para análise da conectividade em Natal-RN:

  - Número de Componentes Conectados: Mede o número total de subgrafos conectados.
  - Tamanho do Maior Componente Conectado: Mede quantos nós estão conectados no maior componente.
  - Comprimento Médio do Caminho Mais Curto: Calcula o caminho mais curto médio entre pares de nós no maior componente.
  - Diâmetro da Rede: Calcula a maior distância entre pares de nós no maior componente.
  - Coeficiente de Aglomeração: Mede a conectividade entre os vizinhos de cada nó.
  - Comprimento do Caminho Mais Curto entre Dois Pontos: Calcula a distância total entre dois pontos específicos em Natal-RN.
  - Ciclos na Rede: Calcula o número de ciclos simples no maior componente conectado.
  - Caminho Mais Curto entre Pontos Específicos
  - Este projeto também inclui a identificação do caminho mais curto entre dois pontos específicos em Natal-RN:

   - Ponto de origem: Cidade Jardim
   - Ponto de destino: Escola de Ciências e Tecnologia (ECT) da UFRN
   - O caminho é visualizado no grafo com destaque.

## Resultados e Análise
* Visualização
* O grafo de Natal-RN e o caminho mais curto entre os pontos (Shopping Cidade Jardim até a Escola de Ciências e Tecnologia (ECT)) são visualizados, com o trajeto destacado para melhor compreensão.

## Interpretação das Métricas
- Número de Componentes Conectados: Indica a quantidade de sub-redes na área de estudo.
- Tamanho do Maior Componente: Mostra a extensão da maior rede conectada, representando a maior parte das conexões possíveis.
- Comprimento Médio do Caminho Mais Curto: Informa a eficiência de deslocamento médio na rede.
- Diâmetro: A distância máxima entre pares indica a acessibilidade em termos de alcance mais longo possível.
- Coeficiente de Aglomeração: Avalia o grau de interconexão local na rede.
- Ciclos: Mostra o número de rotas cíclicas na rede, importante para alternativas de trajeto.
- Repositório e Vídeo Explicativo
- O repositório inclui:
