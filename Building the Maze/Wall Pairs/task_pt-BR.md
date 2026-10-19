Uma parede separa um par de células nas direções N-S ou L-O.
Quando uma célula tem uma parede `"S"` e uma célula adjacente ao sul, então a célula adjacente 
deve ter uma parede `"N"`, que é, essencialmente, a mesma parede. No entanto, em nosso código, 
precisamos criar essa conexão para garantir que, quando removermos uma parede `"S"` de uma célula 
que tem um vizinho `"S"`, o vizinho perca automaticamente sua parede `"N"` 
(e não alguma outra parede!).

Armazenaremos informações sobre as paredes correspondentes no dicionário `wall_pairs`, 
que é um atributo de classe porque esse relacionamento deve ser verdadeiro para todas as instâncias 
da classe `Cell`.

### Tarefa

Adicione pares de parede ausentes (pares `chave:valor`) ao dicionário `wall_pairs`. Os primeiros 
dois pares já foram definidos.