Durante o processo de criação do labirinto, todas as células do labirinto precisam ser visitadas, então, no final, não deve haver células restantes com todas as quatro paredes intactas. Portanto, em algum momento, precisaremos verificar se uma célula ainda tem todas as suas paredes para descobrir quais células podemos visitar em seguida.

### Tarefa

Vamos definir um método que verificará se todos os valores no dicionário `self.walls` são `True`.

<div class="hint">Você poderia tentar usar a função <a href="https://docs.python.org/3/library/functions.html#all"><code>all</code></a> embutida.</div>

### Execute
Execute `output.py` para ver se você implementou o método com sucesso. Deve imprimir `True` se a célula tiver todas as paredes e `False` caso contrário. Também desenhará uma imagem de uma célula (`cell_walls.png`). Tente definir uma das paredes como `False` e executar `output.py` para garantir que ela não esteja lá. Note que, para passar no teste desta tarefa, você precisará definir as 4 paredes de volta para `True` depois de concluir a visualização.