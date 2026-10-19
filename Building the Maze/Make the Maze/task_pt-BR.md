Agora, vamos finalmente juntar tudo e construir o labirinto!

O algoritmo deve produzir um caminho visitando cada célula de acordo com o seguinte procedimento:
1) O algoritmo começa em uma célula dada <code><span style="white-space: nowrap">(0, 0)</span></code> e a marca como visitada. Para manter o controle das células visitadas, usaremos uma lista `cell_stack`.
2) O algoritmo inspeciona as células vizinhas e verifica se alguma delas ainda precisa ser visitada (se tiverem todas suas paredes).
3) Se sim, escolhe uma aleatoriamente e se move até ela, removendo assim a parede entre as células.
4) O algoritmo marca a nova célula atual como visitada (adiciona ao stack).
5) Incrementa o contador das células visitadas.
6) Se a célula atual não tem nenhum vizinho que ainda não foi visitado, recuamos até encontrar uma célula no stack que tenha um vizinho não visitado.
7) O algoritmo termina quando não há mais células não visitadas (o loop `while` garante isso).

Alteramos o `status` da primeira e da última célula visitada em nosso código para fins de visualização.

<details>

Note que `__make_maze` é um método privado. Um [método privado](https://docs.python.org/3/tutorial/classes.html#private-variables) é um método que não deve ser acessado fora da classe nem por qualquer classe base. Em Python, você pode definir um método privado prefixando o nome do método com `__`.
</details>

### Tarefa

Implemente os passos de 3 a 6 descritos acima.

<div class='hint'>Você pode querer usar o método da lista <code>pop()</code> para o passo de retração. Ou talvez você encontre outra maneira!</div>

<div class='hint'>Você pode usar a função <a href="https://docs.python.org/3/library/random.html#random.choice"><code>choice()</code></a> do módulo <code>random</code> (já importado!) para selecionar uma célula vizinha para mover-se a partir da lista de vizinhos válidos.</div>

### Executar

O módulo `output.py` produz uma imagem PNG do seu labirinto. Para verificar a implementação do seu algoritmo de geração de labirintos, sugerimos rodar seu código e visualizar o arquivo `maze.png`.