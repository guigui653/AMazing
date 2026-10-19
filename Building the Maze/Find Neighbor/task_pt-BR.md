Para visitar todas as células da grade, precisamos ser capazes de encontrar os vizinhos da célula atual que ainda têm todas as suas paredes (essas células ainda não foram visitadas!).

O método `find_valid_neighbors` da classe `Maze` aceita um objeto célula e retorna uma lista de objetos célula, que são seus vizinhos válidos. Para determinar quais vizinhos são 'válidos' (neste caso - os que ainda têm todas as suas paredes), precisamos verificar todos os deslocamentos possíveis (definidos na variável `delta`) a partir desta célula e atribuir as coordenadas do vizinho potencial da célula atual mais o delta. Em seguida, verificamos se as coordenadas resultantes realmente estão dentro da nossa grade (no intervalo de `0` a `nx` / `ny`), e se sim, obtemos uma célula nessas coordenadas e verificamos se ela tem todas as suas paredes (anteriormente definimos métodos para essas duas operações). Se o vizinho potencial tem todas as suas paredes, nós o adicionamos à lista que será retornada pelo método.

### Tarefa
Implemente o método `find_valid_neighbors` da classe `Maze` conforme descrito acima.

### Executar
Você pode executar o output.py para ver como o seu código funciona – ele deve desenhar uma imagem PNG (`neighbors.png`) de uma grade com a célula selecionada destacada em preto e seus vizinhos válidos destacados em vermelho. Note que um dos vizinhos não está destacado – está certo, este não é 'válido', pois removemos uma parede entre ele e a nossa célula.

<div class="hint">

Você precisará adicionar informações sobre a `direction` dos vizinhos válidos à lista também, de modo que, no final, ela consista em tuplas como, por exemplo, `('N', <cell.Cell object at 0x114a73580>)`.
</div>