Outro passo crucial é encontrar todas as células adjacentes. Em nosso paradigma, a célula ao norte da atual (se presente) tem um deslocamento de `-1` ao longo do eixo y e um deslocamento de `0` ao longo do eixo x. Ou seja, um vizinho ao norte teria um deslocamento `(0, -1)`.

### Tarefa
Sua tarefa é completar a variável de classe `delta` da `Maze` para que ela contenha todos os deslocamentos possíveis.

<div class="hint">Você precisa adicionar <code>"W"</code> e <code>"E"</code>.</div>