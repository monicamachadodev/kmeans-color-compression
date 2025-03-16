# K-means para Compressão de Cores

## Visão Geral

Este projeto demonstra o uso do algoritmo **K-means** para compressão de cores em imagens. 
> O objetivo é reduzir o número de cores de uma imagem, agrupando pixels semelhantes e substituindo-os por cores representativas.

Isso permite simplificar imagens sem perder significativamente sua qualidade visual.

## Compreensão do Problema

As imagens digitais geralmente contêm uma grande quantidade de cores. Para reduzir essa complexidade, podemos usar **K-means clustering** para agrupar cores semelhantes e substituir os pixels pelas cores centrais de cada cluster. Essa técnica tem aplicações em compressão de imagens, redução de ruído e segmentação de imagens.

## Compreensão dos Dados

A imagem utilizada no projeto é uma fotografia de tulipas. Cada pixel da imagem pode ser representado como um ponto no espaço de cores RGB (Red, Green, Blue), formando um conjunto de dados tridimensional.

**O projeto segue as seguintes etapas:**

- Carregamento da imagem: A imagem original é carregada e convertida em uma matriz de pixels.

- Normalização dos dados: Os valores RGB são normalizados para facilitar o processamento.

- Aplicando K-means: O algoritmo é treinado para agrupar as cores em **k clusters**.

- Reconstrução da imagem: Cada pixel é substituído pela cor do centro do cluster ao qual pertence.

- Avaliação: A qualidade da compressão é analisada comparando imagens geradas com diferentes valores de **k**.

## Exemplo de Compressão de Cores

Aqui está um exemplo de compressão de cores usando **K-means**: Essa fotografia tem 320 pixels verticais e 240 pixels horizontais.

| Imagem Original | K=3 | K=5 | K=10 |
|---|---|---|---|
| ![Original](images/tulipa.jpg) | ![K=3](images/tulipa_k3.jpg) | ![K=5](images/tulipa_k5.jpg) | ![K=10](images/tulipa_k10.jpg) |

Podemos ver que, à medida que **K aumenta**, a imagem se aproxima mais da original, mantendo menos cores distintas.

## Resultados

- A imagem final possui um conjunto reduzido de cores, mantendo a aparência visual similar à original.

- O ajuste de **k** impacta diretamente na qualidade e no nível de detalhe da imagem comprimida.

- O método pode ser usado para outras aplicações como segmentação de imagens e compressão de arquivos.

## Conclusão

Este projeto demonstra como o **K-means** pode ser usado para reduzir a quantidade de cores em uma imagem, mantendo sua estrutura visual. O experimento também mostra como a escolha do valor de **k** afeta a qualidade da compressão.

##  Próximos Passos

- Testar com diferentes tipos de imagens.

- Comparar **K-means** com outros algoritmos de segmentação de imagens.

- Implementar métricas quantitativas para avaliar a perda de informação.

## Requisitos

- *Linguagem:* `Python`

- *Bibliotecas:* `numpy`, `pandas`, `matplotlib`, `scikit-learn`

## Como Executar o Projeto

Clone este repositório:
```bash
git clone https://github.com/monicamachadodev/kmeans-color-compression.git
```
Instale as dependências:
```bash
pip install -r requirements.txt
```
Execute o notebook no Jupyter Notebook ou Google Colab.

##  Contato

Caso tenha dúvidas ou sugestões, fique à vontade para entrar em contato!

