## Logica

### if, else if, else

- if, else if e else sao usados para a logica e manipulacao de dados, como qualquer outra linguagem

_estrutura: if condicao {} else if condicao {} else {}_

```go
if x > 10 {
  fmt.Println("x eh maior que 10")
}
else if x < 10{
  fmt.Println("x eh menor que 10")
}
else{
  fmt.Println("x eh igual a 10")
}
```

### for

- o for do go se parece com o for do java, mas ele eh mais versatil

_estrutura: palavra reservada (for), variavel := valor inicial; condicao do for; oq fazer com a variavel depois de rodar o loop uma vez {}_

```go
for i := 0; i < 5; i++ {
  fmt.Println(%d, i)
}
```

- podemos usar o for para iterar em slices e arrays

_estrutura: palavra reservada (for), variavel atribuida ao INDEX, variavel atribuida ao VALOR do INDEX, :=, palavra reservada (range), nome do array/slice {}_
```go

for index, valor := range arr {
	fmt.Printf("arr[%d] = %d\n", index, valor)
	soma += valor
	}
```

### defer

- defer e uma linha de codigo que roda apos o loop dar um return, nao importa em que lugar do codigo ele esteja

_estrutura: palavra reservada (defer), linha de codigo_

```go
func Defer() {
	defer fmt.Println("Esta mensagem será impressa por último (defer)")
	fmt.Println("Esta mensagem será impressa primeiro")
	fmt.Println("Esta mensagem será impressa segundo")
}
```

### switches

- no go o switch nao precisa necesariamente funcionar em cima da mesma variavel, posso usar condicoes completamente diferentes pno switch

- fallthrough eh utilizado para continuar a logica do switch, mesmo se ele ja tenha caido na condicao

_estrutura: palavra reservada (switch) variavel, {palavra reservada (case), condicao: logica, etc }

```go
func swt(x int){
  switch x {
	  case 0:
		  fmt.Println("Zero")
	  case 1:
		  fmt.Println("Um")
	  case 2:
		  fmt.Println("Dois")
    case 3:
      fmt.Println("Tres")
      fallthrough
    case 4:
      fmt.Println("o numero anterior era 3, e essa mensagem veio de um fallthrough")
    default:
		  fmt.Println("Outro número")
	}
}
```
