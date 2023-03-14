# Variáveis em Python
As variáveis em Python são usadas para armazenar valores, como números, textos, listas, dicionários, objetos e outros tipos de dados. As variáveis em Python são dinamicamente tipadas, ou seja, não é necessário declarar seu tipo explicitamente e elas podem mudar de tipo durante a execução do programa.

## Declaração de variáveis
Em Python, a declaração de variáveis é feita de forma simples, basta atribuir um valor a uma variável. O operador de atribuição em Python é o sinal de igual (=).

```python
# Declaração de uma variável
x = 10
```

## Tipos de variáveis
Em Python, existem os seguintes tipos de variáveis:

- int: [Número inteiro](https://pt.wikipedia.org/wiki/Inteiro);
- float: [Número real](https://pt.wikipedia.org/wiki/N%C3%BAmero_real);
- str: [Texto](https://pt.wikipedia.org/wiki/Texto) (string);
- bool: [Booleano](https://pt.wikipedia.org/wiki/Booleano) (True ou False);

Veja um exemplo de declaração de variáveis com diferentes tipos:

```python
# Declaração de variáveis com diferentes tipos
x = 10 # int
y = 10.5 # float
z = "Olá, mundo!" # str
w = True # bool
```
## Atribuindo tipos de variáveis
Você pode especificar o tipo de uma variável ao atribuir um valor a ela.

```python
x = str(10) # x receberá o valor "10" (string)
y = int(10) # y receberá o valor 10 (inteiro)
z = float(10) # z receberá o valor 10.0 (real)
```

## Aspas simples e duplas
Você pode usar aspas simples ou duplas para declarar uma variável do tipo string.

```python
x = 'Olá, mundo!'
y = "Olá, mundo!"
```

## Maísculas e minúsculas
Em Python, as variáveis são case-sensitive, ou seja, diferenciam maiúsculas de minúsculas.

```python
x = 10
X = 20

print(x) # 10
print(X) # 20
```

## Atribuição múltipla
Em Python, é possível atribuir um mesmo valor a várias variáveis em uma única linha de código.

```python
# Atribuição múltipla
x = y = z = 10
```

## Atribuição de valores a várias variáveis
Em Python, é possível atribuir valores a várias variáveis em uma única linha de código.

```python
# Atribuição de valores a várias variáveis
x, y, z = 10, 20, 30
```

## Atribuição de valores a várias variáveis com tipos diferentes
Em Python, é possível atribuir valores a várias variáveis em uma única linha de código, especificando o tipo de cada variável.

```python
# Atribuição de valores a várias variáveis com tipos diferentes
x, y, z = "Olá", 10, 10.5
```

## Descobrindo o tipo de uma variável
Em Python, você pode descobrir o tipo de uma variável usando a função `type()`.

```python
x = 10
y = "Olá, mundo!"
z = 10.5

print(type(x)) # int
print(type(y)) # str
print(type(z)) # float
```
> [O que é uma função?](funcoes.md)

## Usando input() para receber dados do usuário
Em Python, você pode usar a função `input()` para receber dados do usuário e atribuir a uma variável.

```python
# Usando input() para receber dados do usuário
nome = input("Digite seu nome: ")
print("Olá, " + nome)
```
> [Aprenda mais sobre a função input()](funcoes.md#input)

## Variáveis globais
Variáveis globais são variáveis que podem ser acessadas de qualquer parte do programa.

```python
# Variável global
x = 10

def funcao():
    print(x)

funcao() # 10
```

## Variáveis locais
Variáveis locais são variáveis que só podem ser acessadas dentro da função onde foram declaradas.

```python
# Variável local
def funcao():
    x = 10
    print(x)

funcao() # 10
print(x) # NameError: name 'x' is not defined
```

## Variáveis de instância
Variáveis de instância são variáveis que pertencem a uma instância de uma classe.

```python
# Variável de instância
class Pessoa:
    def __init__(self, nome):
        self.nome = nome

pessoa = Pessoa("João")
print(pessoa.nome) # João
```
> [O que é uma classe?](classes.md)

## Variáveis de classe
Variáveis de classe são variáveis que pertencem a uma classe.

```python
# Variável de classe
class Pessoa:
    contador = 0

    def __init__(self, nome):
        self.nome = nome
        Pessoa.contador += 1

pessoa1 = Pessoa("João")
pessoa2 = Pessoa("Maria")
print(Pessoa.contador) # 2
```

## Variáveis estáticas
Variáveis estáticas são variáveis que pertencem a uma classe e são compartilhadas por todas as instâncias da classe.

```python
# Variável estática
class Pessoa:
    contador = 0

    def __init__(self, nome):
        self.nome = nome
        Pessoa.contador += 1

pessoa1 = Pessoa("João")
pessoa2 = Pessoa("Maria")
print(Pessoa.contador) # 2
```

## Variáveis de instância privadas
Variáveis de instância privadas são variáveis que pertencem a uma instância de uma classe e só podem ser acessadas dentro da classe.

```python
# Variável de instância privada
class Pessoa:
    def __init__(self, nome):
        self.__nome = nome

    def get_nome(self):
        return self.__nome

pessoa = Pessoa("João")
print(pessoa.get_nome()) # João
print(pessoa.__nome) # AttributeError: 'Pessoa' object has no attribute '__nome'
```

## Variáveis de classe privadas
Variáveis de classe privadas são variáveis que pertencem a uma classe e só podem ser acessadas dentro da classe.

```python
# Variável de classe privada
class Pessoa:
    __contador = 0

    def __init__(self, nome):
        self.nome = nome
        Pessoa.__contador += 1

    def get_contador(self):
        return Pessoa.__contador

pessoa1 = Pessoa("João")
pessoa2 = Pessoa("Maria")
print(pessoa1.get_contador()) # 2
print(Pessoa.__contador) # AttributeError: type object 'Pessoa' has no attribute '__contador'
```

## Variáveis estáticas privadas
Variáveis estáticas privadas são variáveis que pertencem a uma classe e são compartilhadas por todas as instâncias da classe, e só podem ser acessadas dentro da classe.

```python
# Variável estática privada
class Pessoa:
    __contador = 0

    def __init__(self, nome):
        self.nome = nome
        Pessoa.__contador += 1

    def get_contador(self):
        return Pessoa.__contador

pessoa1 = Pessoa("João")
pessoa2 = Pessoa("Maria")
print(pessoa1.get_contador()) # 2
print(Pessoa.__contador) # AttributeError: type object 'Pessoa' has no attribute '__contador'
```

## Variáveis de instância protegidas
Variáveis de instância protegidas são variáveis que pertencem a uma instância de uma classe e só podem ser acessadas dentro da classe e de suas subclasses.

```python
# Variável de instância protegida
class Pessoa:
    def __init__(self, nome):
        self._nome = nome

    def get_nome(self):
        return self._nome

class Aluno(Pessoa):
    def __init__(self, nome, matricula):
        super().__init__(nome)
        self.matricula = matricula

aluno = Aluno("João", 123)
print(aluno.get_nome()) # João
print(aluno._nome) # João
```

## Variáveis de classe protegidas
Variáveis de classe protegidas são variáveis que pertencem a uma classe e só podem ser acessadas dentro da classe e de suas subclasses.

```python
# Variável de classe protegida
class Pessoa:
    _contador = 0

    def __init__(self, nome):
        self.nome = nome
        Pessoa._contador += 1

    def get_contador(self):
        return Pessoa._contador

class Aluno(Pessoa):
    def __init__(self, nome, matricula):
        super().__init__(nome)
        self.matricula = matricula

aluno = Aluno("João", 123)
print(aluno.get_contador()) # 1
print(Pessoa._contador) # 1
```

### Conclusão
Neste capítulo, você aprendeu sobre variáveis e seus tipos, e também sobre as diferentes formas de declarar variáveis em Python.

## Próximo capítulo
[Operadores](operadores.md)

## Capítulos anteriores
- [Capítulo 1 - Introdução](README.md)
- [Sintaxe](sintaxe.md)
- [Comentários](comentarios.md)