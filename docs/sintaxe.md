# Sintaxe do Python
A sintaxe do Python é relativamente simples e fácil de aprender, com destaque para a estrutura de identação que é utilizada no lugar de chaves, como é comum em outras linguagens de programação. Aqui estão alguns exemplos de sintaxe em Python:

## Declaração de variáveis
Em Python, não é necessário declarar variáveis antes de usá-las. Basta atribuir um valor a uma variável e ela será criada. O tipo da variável é determinado automaticamente quando você atribui um valor a ela.
```python
# Declaração de uma variável inteira
x = 10

# Declaração de uma variável de texto
nome = "João"

# Declaração de uma variável booleana
ativo = True
```
> [Veja mais sobre variáveis](variaveis.md)
## Comentários
Comentários são usados para explicar o código, e são ignorados pelo interpretador Python. Comentários começam com o símbolo #, e podem ser colocados em qualquer lugar na linha.
```python
# Este é um comentário
print("Hello, World!") # Este é um comentário
```
## Identação
Identação é usada em Python para definir blocos de código. O número de espaços é irrelevante, mas deve ser consistente. Normalmente, 4 espaços são usados para identação, e é recomendado que você use a mesma quantidade de espaços em todo o seu código.
```python
# Exemplo de identação incorreta
if 5 > 2:
print("Python funciona!")
```
```python
# Exemplo de identação correta
if 5 > 2:
    print("Python funciona!")
```
## Linhas em branco
Linhas em branco são usadas para separar funções e classes, e também para separar blocos de código dentro de funções e classes. Em geral, você deve usar uma linha em branco para separar funções e classes, e duas linhas em branco para separar blocos de código dentro de funções e classes.
```python
# Exemplo de duas linhas em branco
class MyClass:
    x = 5

    def __init__(self):
        pass

    def myfunc(self):
        print("Hello, World!")
```
## Linhas de código longas
Se você tiver uma linha de código que seja muito longa, você pode dividí-la em duas ou mais linhas com o caractere de barra invertida \.
```python
# Exemplo de linha de código longa
x = 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10 + 11 + 12 + 13 + 14 + 15 + 16 + 17 + 18 + 19 + 20
```
```python
# Exemplo de linha de código longa dividida em duas linhas
x = 1 + 2 + 3 + 4 + 5 + 6 + 7 + 8 + 9 + 10 + 11 + 12 + 13 + 14 + 15 + 16 + 17 + 18 + 19 + \
    20
```
## Condicionais
Em Python, a declaração if é usada para condicionais.
```python
# Estrutura condicional simples
if x > 5:
    print("x é maior que 5")
else:
    print("x é menor ou igual a 5")

# Estrutura condicional com elif
if x > 10:
    print("x é maior que 10")
elif x == 10:
    print("x é igual a 10")
else:
    print("x é menor que 10")
```
## Laços de repetição (loops)
Em Python, existem dois tipos de laços de repetição: for e while.
```python
# Loop while
i = 0
while i < 10:
    print(i)
    i += 1

# Loop for
for i in range(0, 10):
    print(i)
```
## Funções
Funções são usadas para executar tarefas específicas. Elas podem receber parâmetros e retornar um valor.
```python
# Declaração de uma função
def soma(a, b):
    return a + b

# Chamada da função
resultado = soma(10, 5)
print(resultado)
```
## Listas
Listas são usadas para armazenar vários itens em uma única variável.
```python
# Declaração de uma lista
nomes = ["João", "Maria", "Pedro", "Lucas"]

# Acesso aos elementos da lista
print(nomes[0])
print(nomes[1])
print(nomes[-1]) # último elemento da lista

# Adição de elementos à lista
nomes.append("Ana")
```
## Classes
Classes são usadas para criar novos tipos de objetos.
```python
# Declaração de uma classe
class Pessoa:
    def __init__(self, nome, idade):
        self.nome = nome
        self.idade = idade

    def saudacao(self):
        print(f"Olá, meu nome é {self.nome} e eu tenho {self.idade} anos.")

# Criação de um objeto
pessoa1 = Pessoa("João", 30)

# Chamada do método da classe
pessoa1.saudacao()
```