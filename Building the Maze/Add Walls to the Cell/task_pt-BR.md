Células em nosso labirinto podem ter um número variável de paredes (até 4) separando-as das células vizinhas. 
Apenas células que compartilham uma parede são consideradas vizinhas, células adjacentes na diagonal não são.


Precisamos ser capazes de acompanhar as paredes presentes. Uma solução fácil seria manter um dicionário 
de paredes para cada objeto célula, onde cada chave (parede) está associada a um valor (`True`/`False`, dependendo 
de se está presente ou ausente). Em nosso programa, cada célula começa com todas as quatro paredes (`"N"`, `"S"`, `"E"`, `"W"`) 
no lugar. Mais adiante, removeremos algumas dessas paredes.

### Tarefa

Vamos criar um dicionário `paredes` onde as chaves são direções (`"N"`, `"S"`, `"E"` e `"W"`) e os valores são 
booleanos, com o valor `True` quando a parede existe e `False` caso contrário. Inicialmente, todas as células têm 
todas as quatro paredes.

### Executar
Execute `output.py` para ver se você adicionou com sucesso as paredes à célula. Se sim, ele gerará um arquivo PNG 
(`cell_walls.png`) com a imagem de uma célula com 4 paredes! Clique duas vezes no arquivo para ver a imagem.