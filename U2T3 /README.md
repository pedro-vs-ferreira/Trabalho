# Algoritmo de Dijkstra Aplicado a Pontos de Interesse em Natal-RN

Este projeto implementa o algoritmo de Dijkstra para calcular as rotas mais curtas entre diversos pontos de interesse na cidade de Natal-RN. Utiliza a biblioteca `OSMnx` para obter e visualizar o grafo da rede viária e `networkx` para a execução do algoritmo.

## Pontos de Interesse

Os seguintes locais foram considerados como pontos de interesse:

- **Minha Casa**: `-5.800599508947651, -35.206925674334684`
- **Midway**: `-5.810896030636198, -35.206348200159326`
- **Casa da Namorada**: `-5.809421534902807, -35.2016377950458`
- **DCA**: `-5.842870143233271, -35.197310236740044`
- **ECT**: `-5.843378581884456, -35.19939757290338`
- **Casa de Vó**: `-5.819847884661806, -35.21167141270225`
- **Empresa**: `-5.7826047930669215, -35.20486484624309`

## Pares de Origem e Destino

As rotas são calculadas entre os seguintes pares de origem e destino:

1. Minha Casa -> Midway
2. Midway -> Casa da Namorada
3. Casa da Namorada -> DCA
4. DCA -> ECT
5. ECT -> Casa de Vó
6. Casa de Vó -> Empresa
7. Empresa -> Minha Casa
8. DCA -> Empresa
9. Midway -> ECT
10. Minha Casa -> Casa de Vó

## Imagens dos Grafos

### 1. Minha Casa -> Midway
![Minha Casa -> Midway](images/grafo1.png)

### 2. Midway -> Casa da Namorada
![Midway -> Casa da Namorada](images/grafo2.png)

### 3. Casa da Namorada -> DCA
![Casa da Namorada -> DCA](images/grafo3.png)

### 4. DCA -> ECT
![DCA -> ECT](images/grafo4.png)

### 5. ECT -> Casa de Vó
![ECT -> Casa de Vó](images/grafo5.png)

### 6. Casa de Vó -> Empresa
![Casa de Vó -> Vesthosp](images/grafo6.png)

### 7. Empresa -> Minha Casa
![Vesthosp -> Minha Casa](images/grafo7.png)

### 8. DCA -> Empresa
![DCA -> Vesthosp](images/grafo8.png)

### 9. Midway -> ECT
![Midway -> ECT](images/grafo9.png)

### 10. Minha Casa -> Casa de Vó
![Minha Casa -> Casa de Vó](images/grafo10.png)

