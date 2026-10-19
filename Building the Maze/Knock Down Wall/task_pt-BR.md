Para criar um labirinto a partir de uma grade de células desconectadas, precisamos eliminar muitas paredes. Começaremos a partir da célula em <code><span style="white-space: nowrap">(0, 0)</span></code> e percorreremos a grade. Sempre que uma nova célula for visitada, a parede entre a nova célula e a anterior é removida. Você pode imaginar algo realmente se movendo de uma célula para outra e derrubando as paredes fisicamente.

Além disso, todas as células precisam ser visitadas pelo menos uma vez para que nenhuma delas tenha todas as quatro paredes em pé quando o algoritmo terminar.

### Tarefa

Nesta tarefa, vamos implementar o método `knock_down_wall` da classe `Cell`. Ele aceita duas células – uma célula atual (`self`) e sua vizinha (`other`) para a qual vamos nos mover, bem como a `wall` entre elas. Primeiro, o método remove a `wall` da célula atual definindo-a como `False`. Em seguida, precisamos remover (definir como `False`) a parede correspondente da célula `other`. A função deve escolher a parede adequada usando o dicionário previamente criado `wall_pairs`.

<div class='hint'>Acesse a parede necessária da célula <code>other</code> pesquisando <code>wall</code> em <code>wall_pairs</code> da classe <code>Cell</code>.</hint>

### Executar
Execute `output.py` para ver se você implementou com sucesso o método. Ele desenhará duas imagens de duas células (`adjacent_cells.png` e `removed_NS_wall.png`). A primeira mostra as células antes de uma parede ser derrubada, e a segunda – depois. O código também imprime o dicionário `walls` para cada célula.