#### Pré-requisitos do curso

Conhecimento básico de Python:
- Operações Básicas
- Loops
- Estruturas de Dados
- Funções
- Classes

Se você não conhece esses conceitos, pode querer conferir primeiro nosso curso [Introdução ao Python](https://plugins.jetbrains.com/plugin/16630-introduction-to-python).

#### Algoritmo DFS

Neste projeto, vamos gerar um labirinto 2D usando um algoritmo que trata um labirinto completo como uma [árvore](https://en.wikipedia.org/wiki/Tree_(data_structure)), onde os ramos representam caminhos através do labirinto. Este algoritmo é chamado de [Busca em Profundidade](https://en.wikipedia.org/wiki/Depth-first_search) (DFS). DFS começa no nó raiz e explora o máximo possível ao longo de cada ramo antes de retroceder. A busca lembra dos nós visitados anteriormente e não os repete. Isso é importante porque realizar a mesma busca sem lembrar dos nós visitados resulta em um loop infinito.

#### O que é um labirinto?

Em duas dimensões, um labirinto é uma série de caminhos separados por paredes, e para simplificar, pode-se pensar nele como uma grade bi-dimensional de células. Cada célula é um ponto na grade que pode ter até 4 vizinhos: ao norte, leste, sul ou oeste. Uma célula pode ser separada de seus vizinhos por paredes. Se uma célula, por exemplo, tem um vizinho a leste e há uma parede entre eles, então este vizinho certamente tem uma parede a oeste (é a mesma parede).

![img](maze_example.png)

#### Descrição do Problema

Começaremos com uma grade $N * N$ onde todas as células têm todas as quatro paredes ("N", "S", "E", "W"). Para ir de uma grade de células desconectadas a um labirinto, precisaremos derrubar algumas delas. Quando uma nova célula é visitada pelo algoritmo, a parede entre a nova célula e a anterior é removida.

O algoritmo que vamos escrever deve produzir um caminho visitando cada célula da grade de acordo com as seguintes regras:
- Começar em uma célula determinada e marcá-la como visitada.
- Se alguma das células vizinhas ainda não foi visitada, escolha uma delas aleatoriamente, mova-se para ela e remova a parede entre as duas células.
- Se todos os vizinhos já foram visitados, volte para a última célula com um vizinho não visitado.

Uma vez que não há mais células não visitadas – o labirinto está construído, e o algoritmo termina.