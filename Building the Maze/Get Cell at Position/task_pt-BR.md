Ao construir o labirinto célula por célula, precisaremos iterar sobre as células por suas coordenadas. Para iterar sobre objetos células, utilizaremos o método `cell_at` da classe `Maze`, que retornará uma `Cell` na posição especificada.

> Para acessar o elemento `b` em uma matriz 3 x 3 `my_array`, que se parece com `[[a, b, c], [d, e, f], [g, h, i]]`, você precisa usar primeiro seu índice de linha e depois seu índice de coluna: `my_array[0][1]`.

### Tarefa
Implemente uma função que aceite coordenadas `(x, y)` e retorne um objeto `Cell` naquela posição.

<div class='hint'>Acesse a célula através de <code>maze_grid</code>.</div>

### Execução
Você pode testar como seu método `cell_at` funciona executando `output.py` e selecionando uma célula que deseja que seja destacada. Será desenhada uma imagem PNG da grade do tamanho especificado com a célula selecionada destacada em preto (`highlighted_cell.png`).