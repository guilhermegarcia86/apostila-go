
# Golang

## [História](#Historia)
## [Instalação](#Instalação)
## [Estrutura](#Estrutura)
## [Visibilidade](#Visibilidade)
## [Variáveis e Constantes](#Var_e_Const)
## [Tipos Básicos](#DataTypes)
## [Operadores](#Operadores)

# Instalação

[Passos para instalação](https://golang.org/doc/install)

# Estrutura

```go

package main

import "fmt"

func main(){
    fmt.Printf("Hello word")
}
```

Os arquivos .go devem iniciar com a definição de pacote (_package_) que não exige, como em outras linguagens que seja o mesmo nome do arquivo mas é uma boa prática deixar os nomes iguais.
Após temos as definiçções de importações com a palavra _import_ que pode ser definada como um bloco quando temos multiplos pacotes importados exemplo:

```go
import (
    "fmt"
    "net"
)
```

E seguido das funções variáveis e etc.

# Visibilidade

A visibilidade em **GO** é definida por convenções, como muitas coisas nessa linguagem, e para visibilidade de **structs**, **functions**, **variaveis**, **contantes** e etc é usado a seguinte convenção, tudo o que começar com letra maiúscula será público e tudo o que começar com letra minúscula será privado, exemplo:

```go
func functionprivada(){
// função privada
}

func FunctionPublica(){
// função pública
}
```

# Variáveis e Constantes

Podemos declarar as variáveis com a palavra _var_ seguida do tipo e seu valor:
```go
var num int32 = 42
```
E contantes da mesma forma com a palavra reservada _const_:
```go
const PI float64 = 3.1415
```
Temos também a opção de iniciarmos blocos de variávies e constantes:
```go
var (
    a = 3
    b = 4
)
const (
    c = 5
    d = 6
)
```
Apesar das duas abordagens serem simples o mais comum é não tipar as variáveis e constantes já que o **GO** nos provê inferência de tipos automaticamente:
```go
num := 42
```
Com operador ":=" é o que faz a inferência de tipos automáticamente, isso que dizer que o tipo é definido de forma automática. Porém como o **_GO_** é uma linguagem fortemente tipada não podemos mudar o tipo de variável após a sua declaração.

# Tipos Básicos
Os tipos básicos da linguagem:

bool _booleano_

string 

int  int8  int16  int32  int64
uint uint8 uint16 uint32 uint64 uintptr (tipos numéricos)

byte // alias for uint8

rune // alias for int32
     // represents a Unicode code point

float32 float64 (pontos flutuantes)

complex64 complex128

# Operadores

## Atrbibuição
```go
func main() {

    num := 42
    num += 42
    num -= 42
    num /= 42
    num *= 42
    num %= 42

```

## Aritméticos
```go
func main() {   
    a := 3   
    b := 2   
    
    Soma => a+b   
    Subtração => a-b   
    Divisão => a/b   
    Multiplicação => a*b   
    Mod => a%b
```

## 


