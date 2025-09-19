## Variaveis

### Tipos de variaveis

```
int, int8, int16, int32, int64, uint, uint8, uint16, uint32, uint64, float32, float64, complex64, complex128

bool

string

Arrays, slices, maps, structs, pointers, functions, interfaces, channels.
```

### Variaveis publicas

- em Go, as variaveis publicas comecam com letra Maiuscula, diferente de outras linguagens onde usamos uma palavra reservada para fazer essa distincao

_estrutura das variaveis: palavra reservada (var), nome da variavel, tipo da variavel_

```go
var Insano bool
var Nome, Emal string
var Idade int
var Peso float32
```

### Variaveis privadas

- em Go, as variaveis privadas comecam com letra minuscula, diferente de outras linguagens onde usamos uma palavra reservada para fazer essa distincao

_estrutura das variaveis: palavra reservada (var), nome da variavel, tipo da variavel_

```go
var dormindo bool
var cartao, cpf string
var voosAIndoneia int
var dinheiroNoNubank float32
```

### Structs

- Structs sao similar a objetos, ele armazena variaveis de diversos tipo

_estrutura da Structs: palavra reservada (type), nome da Struct, palavra reservada (Struct), {}_

```go
type User struct {
name string
email string
age int
}
```

### Array

- Arrays tem tamanho fixo, definido na compilacao do projeto, nao crescem, nem dimunuem

_estrutura do array: nome do array, :=, tamanho do array ->[]{item,item,item}_

```go
Arr := [3]int{1,2,3}
```

### Slice

- Slices tem tamanho variavel, podem crescer ou diminuir dependendo da necessidade

_estrutura do slice: nome do slice, :=, []{item,item,item}_

```go
Slc := []{1,2,3}
```
```
