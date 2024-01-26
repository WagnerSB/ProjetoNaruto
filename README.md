# Guess the PIN
Jogo para advinhação de PIN aleatório de 4 ou mais dígitos.

### Tópicos
- [Detalhes](#detalhes)
- [Como utilizar o sistema](#como-utilizar-o-sistema)
- [Dificuldades conhecidas](#dificuldades-conhecidas)
- [Autores](#autores)

## Detalhes
A ideia principal do projeto se resume a uma entrada númerica feita pelo usuário, a qual é válidada e passa por um processo de checagem para verificar se o número informado é o correto, se é menor, muito menor, maior ou muito maior, onde "muito" é definido pela diferença entre o número informado e o correto. Se a diferença for de 20% ou mais do valor máximo total + 1, então o número informado é muito maior ou muito menor. Por exemplo, para um PIN de 4 dígitos, essa diferença é de 2000 pois o número máximo mais um é 10000, e 20% de 10000 é 2000. Também contando com um seletor de dificuldade onde pode ser selecionado o número de dígitos que o PIN possui, indo de 4 até 10.<br>
Para a verificação é utilizado um processo para verificar se o número informado é realmente um inteiro, caso contrário, o dígito é removido do input, dessa maneira permitindo apenas os números a ficarem no input, buscando restringir qualquer possível erro. Dessa forma, mesmo que a seguinte string fosse colada no input "123e .4rfr5", o que realmente apareceria seria: "12345". Além de verificar se foi informado a quantidade mínima de dígitos conforme selecionado pelo usuário.
![Tela de vitória Guess the PIN](src/Imagens/Jiraiya.jpg "Tela de vitória Guess the PIN")

## Como utilizar o sistema
1. O usuário escolhe uma quantidade de dígitos, ou utiliza a predefinição (4 dígitos).
2. Informa um valor, e pressiona o botão "submit" ou a tecla "enter".
3. Recebe um feedback sobre o valor informado.
4. Repetem-se os passos 2 e 3 até que o usuário informe o PIN correto.
5. Pode-se jogar novamente apertando no botão "new game".

## Dificuldades conhecidas
- Fazer a validação para aceitar apenas números devido ao fato de ocorrer um bug quando utilizado o input type="number", então foi alterado para "text".
- Fazer testes e achar possíveis bugs.

## Autores
[Wagner Schröer Bagatini](https://github.com/WagnerSB)
