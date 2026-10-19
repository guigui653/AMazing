É hora de começar a criar nosso labirinto! Como mencionado antes, podemos representar um labirinto como uma grade de células interconectadas de `nx` * `ny`, e ele será construído começando na célula indexada em <code><span style="white-space: nowrap">(0, 0)</span></code>. Primeiro, criaremos a grade propriamente dita e a visualizaremos.

Agora precisaremos de uma nova classe, `Maze`, definida em um módulo separado `maze.py`. O método `__init__()` da classe `Maze` irá inicializar o objeto labirinto, suas dimensões `x` e `y` (medidas em número de células ao longo do eixo correspondente) e a grade do labirinto na forma de um array [NumPy](https://numpy.org/doc/stable/user/whatisnumpy.html).

> Um [array NumPy](https://numpy.org/doc/stable/reference/generated/numpy.array.html) é uma grade de valores (todos do mesmo tipo). É indexado por inteiros não negativos. O número de dimensões é o grau do array (trabalharemos com um array de grau 2); a `shape` de um array é uma tupla de inteiros que indica o tamanho do array ao longo de cada dimensão. Podemos inicializar arrays NumPy a partir de listas aninhadas e acessar elementos usando colchetes.

### Tarefa
Complete a linha do método `__init__()` para inicializar o `maze_grid`.

<div class='hint'>Seria conveniente usar <a href="https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions">compreensão de listas</a>.</div>

### Executar
Execute `output.py` para ver se você implementou o método com sucesso. Ele irá desenhar uma imagem PNG da grade (`maze_grid.png`).