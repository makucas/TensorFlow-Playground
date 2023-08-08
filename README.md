# TensorFlow-Playground
> Projeto desenvolvido durante a disciplina de Inteligência Artificial ministrada pelo professor Lucas Araújo Pereira na Universidade Federal de Goiás. Implementação em Python utilizando Pytorch. 

## Índice

- [Visão Geral](#visão-geral)
- [Implementação](#implementação)
- [Resultados](#resultados)
- [Referências](#referências)
- [Licença](#licença)

## Visão Geral

* Esse projeto tem como objetivo simular o ambiente apresentado em https://playground.tensorflow.org, mais especificamente o problema de Classificação
* Das principais características implementadas:
  * 4 Datasets (Circle, Exclusive OR, Gaussian, Spiral)
  * Split Ratio, Noise e Batch Size
  * 4 Features (x1, x2, x1², x2²)
  * Capacidade de adicionar e remover Nuerônios e Camadas
    
 ![image](https://github.com/makucas/TensorFlow-Playground/assets/46076494/6f097744-3928-4d70-a2d4-11e7d45bbb4f)


## Implementação

* A implementação foi feita em PyTorch visando atender as principáis características citadas no tópico de visão geral.
* Cada conjunto de dados é composto por 800 pontos (com exceção do Exclusive Or que possui apenas 400), possuindo suas cordenadas x,y e a respectiva label indicando a coloração daquele ponto. Vale ressaltar que para os resultados obtidos, o dataset foi dividido em 50% para treino e 50% para teste. 
* O modelo consiste de camadas lineares extraídas da classe nn.Module, e a implementação do mesmo permite adicionar x neurônios e y camadas.
* A Loss utilizada foi a MeanSquareError, e o batch_size foi 10.
* Os conjuntos de dados foram treinados com um número de épocas diferente, que variou de 100 até 1000 épocas, dependendo da complexidade do problema.
  
## Resultados

* Como é possível evidênciar nos gráficos gerados ao final do experimento, a rede aprendeu os 4 conjuntos de dados com uma precisão acima de 99%.
  
![Plots](https://github.com/makucas/TensorFlow-Playground/assets/46076494/c48e1e42-ebda-4d81-8b25-4595e418fbd3)

## Referências
* https://playground.tensorflow.org

## Licença
[MIT](https://choosealicense.com/licenses/mit/)

