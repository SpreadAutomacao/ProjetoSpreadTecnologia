Nesse tutorial vamos falar o básico de Ruby.


1. O padrão de espaçamento entre a funçao deve ser igual a 4 espaços dentro da função, função é nada menos que um bloco de código com uma funcionalidade específica, exemplo:
```ruby
=begin
Pra fazer um comentário grande usamos no inicio do "=begin" e no final do comentário usamos o "=end", sem as aspas duplas.
Um comentário simples em uma linha usamos o jogo da velho/cerquilha #
=end

def nome_da_funcao(string, incrementa=1)
  incrementa += 1
  print(string + incrementa.to_s) 
end

# finalizou_a_funcao_e_voltei_pro_inicio
nome_da_funcao("Valor: ") # fiz a chamada da minha função, nessa linha.

```
O **print** no meu código é a função que vai imprimir o valor no console ou shell/cmd/prompt, a função print é diferente das outras linguagens, pois se colocar o print em baixo ela vai concatenar o resultado de cima com o de baixo. Como no exemplo abaixo.
O comando mais usual no ruby é o **puts** ao invés do print, pois na função puts ela não concatena os valores em sequência, no final ela encerra com um enter "\n".<br>

O **def** é uma definição que aqui vai estar uma função que pode ser retornada ou passada (def vem de function definition).<br>

O **to_s** A função to_s convert o valor numerico para string/texto.<br>

O **+** O simbolo de + concatena os dois valores para exibir no console.<br>

```ruby
=begin
Pra fazer um comentário grande usamos no inicio do "=begin" e no final do comentário usamos o "=end", sem as aspas duplas.
Um comentário simples em uma linha usamos o jogo da velho/cerquilha #
=end

def nome_da_funcao(string, incrementa=1)
  incrementa += 1
  puts(string + incrementa.to_s )
  print(string + incrementa.to_s)
  print(string + incrementa.to_s  + "\n")
end

# finalizou_a_funcao_e_voltei_pro_inicio
nome_da_funcao("Valor: ") # fiz a chamada da minha função, nessa linha.

```
<br><br>

2. No rubymo devemos importar um biblioteca, é regra básica importar as bibliotecas no inicio do seu código. A importação deve ser separada por linhas.

Fazer assim
```ruby
require 'watir'
require 'selenium-webdriver'
```

Segunda forma de fazer a importação, usando o **require_relative**: 
```ruby:
require_relative 'subfolder/meu_arquivo'
```

<br><br>
3. Como trabalhar com condições em ruby, ou seja if, elsif e else.

```ruby

x = 5  # Criei uma variável x que vai receber um valor numerico 5.

# minha primeira condição, verifica se o valor é menor que 4.
if x < 1
    print("valor incorreto!")
elsif x == 4  # minha segunda condição, verifica se o valor é igual a 1.
    print("valor incorreto!")
elsif x >= 5 and x < 10  # minha terceira condição, verifica se o valor é maior e igual a 5 e menor que 10.
    print("O valor esperado está correto!")
else # O else é digamos se nenhuma das condições foi realizada, ele vai entrar nesse bloco de código.
    print("Nenhuma condição foi encontrada!")
end
```   
![alt text](http://diwo.bq.com/wp-content/uploads/2015/10/ifelse.png "Condição IF ELSE")

Tome muito cuidado quando for criar condições somente use quando for preciso, o excesso de condições pode deixar o código lento.

**Abaixo segue uma lista com os operadores aritméticos utilizados em Python:**

```ruby
+   # soma
–   # subtração
*   # multiplicação
/   # divisão
//  # divisão de inteiros
**  # potenciação, dois asteristicos.
%   # módulo (resto da divisão)
```

**Segue também os operadores lógicos:**
```ruby
>   # maior
=   # maior ou igual
<=  # menor ou igual
==  # igual
!=  # diferente
not # Operador lógico que representa a negação (inverso) da variável atual. Se ela for verdade, torna-se falsa, e vice-versa.
and # Operador lógico onde a resposta da operação é verdade se ambas as variáveis de entrada forem verdade.
or  # Operador lógico onde a resposta da operação é verdade se e somente se pelo menos uma das variáveis de entrada for verdade.
```