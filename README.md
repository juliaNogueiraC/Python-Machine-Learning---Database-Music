# Projeto de Machine Learning - Python, sobre um preditor de gênero musical 
A imagem a seguir apresenta uma árvore de decisão para classificar músicas em três gêneros: Acoustic, Dance e HipHop. A árvore é composta por diversos nós, cada um representando uma pergunta ou decisão que leva a uma ramificação diferente. As folhas da árvore, representadas por retângulos, indicam a classificação final da música.

![outfile](https://github.com/juliaNogueiraC/Python-Machine-Learning---Database-Music/assets/69528739/539ec57f-9f8e-4080-b654-7cb004db2c30)


# Detalhes da Árvore:
## Nó Raiz:

- Pergunta: A idade do artista é menor ou igual a 30,5 anos?
- Valor Gini: 0,778 (indica a impureza do conjunto de dados)
- Número de amostras: 18

## Ramo Esquerdo:

- Condição: Idade menor ou igual a 25,5 anos
- Valor Gini: 0,5 (indica um conjunto de dados mais puro)
- Número de amostras: 6
  
### Classificação:
- Se o gênero for masculino (valor <= 0,5): Acoustic
- Se o gênero for feminino (valor > 0,5): Dance
- 
## Ramo Direito:

- Condição: Idade maior que 25,5 anos
- Valor Gini: 0,75 (indica um conjunto de dados mais puro)
- Número de amostras: 12
- 
### Classificação:
- Se o gênero for masculino (valor <= 0,5): HipHop
- Se o gênero for feminino (valor > 0,5): Acoustic
  
## Observações:
- A árvore de decisão utiliza duas variáveis para classificar as músicas: idade do artista e gênero do artista.
- A idade do artista parece ser o fator mais importante na classificação, pois é a primeira pergunta que a árvore faz.
- O gênero do artista é usado para refinar a classificação dentro de cada faixa etária.
- A árvore de decisão foi construída usando um conjunto de dados de 18 músicas.
- O valor Gini é uma medida da impureza do conjunto de dados. Um valor Gini de 0 indica um conjunto de dados puro, enquanto um valor Gini de 1 indica um conjunto de dados completamente impuro.
