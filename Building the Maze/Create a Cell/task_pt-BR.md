O labirinto pode ser representado como uma grade de células. Cada célula do labirinto possui coordenadas 2D únicas <code><span style="white-space: nowrap">(x, y)</span></code>, que definem sua posição dentro da grade e de dois a quatro vizinhos: dois no caso das células de canto, como <code><span style="white-space: nowrap">(1, 1)</span></code> ou <code><span style="white-space: nowrap">(1, 3)</span></code> no exemplo abaixo, e quatro no caso das células internas, por exemplo, <code><span style="white-space: nowrap">(2, 2)</span></code>. Uma célula pode ter paredes nos lados norte, leste, sul ou oeste.

<style>
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
<img src="maze_grid.png" alt="imagem centralizada" width="300">

<details>
<summary>Classes em Python</summary>
<a href="https://docs.python.org/3/tutorial/classes.html">Classes</a> são uma forma prática de definir e armazenar objetos personalizados em Python. Criar uma nova classe cria um novo tipo de objeto, e novas instâncias desse tipo podem então ser criadas. Cada instância de classe pode ter atributos e métodos associados a ela para manter e modificar seu estado. Utilizaremos classes para definir os objetos e funcionalidades necessárias neste curso. Se você não está familiarizado com classes, sugerimos que você confira o curso de <a href="https://plugins.jetbrains.com/plugin/16630-introduction-to-python">Introdução ao Python</a> ou o percurso de Python na <a href="https://hi.hyperskill.org?utm_source=ide&utm_medium=ide&utm_campaign=ide&utm_content=first-task">JetBrains Academy</a> primeiro.
</details>

Neste estágio, vamos simplesmente inicializar uma célula da grade com suas coordenadas. Definimos a classe `Cell` para os objetos de célula do labirinto. Cada célula será uma instância de `Cell`, mas todas terão coordenadas únicas. Portanto, parece apropriado armazenar as coordenadas como [variáveis de instância](https://docs.python.org/3/tutorial/classes.html#class-and-instance-variables).

### Tarefa

Vamos [inicializar](https://docs.python.org/3/tutorial/classes.html#class-objects) uma `Cell` em <code><span style="white-space: nowrap">(x, y)</span></code>.

### Executar

Execute `output.py` para ver a saída impressa da inicialização da célula em <code><span style="white-space: nowrap">(x, y)</span></code>. Para isso, basta clicar com o botão direito no arquivo para que você possa ver o menu de contexto e selecionar Executar ‘output’.

Alternativamente, você pode usar o ícone na margem próximo à instrução `if __name__ == '__main__':` dentro de `output.py`.