Um componente React é uma parte da interface da aplicação que pode ser repetida várias vezes, com informações diferentes.
É uma função que retorna HTML. JSX = JavaScript + XML

CSS Modules utiliza somente classes.

# Key no React

## Por que única?

3 momentos em que um componente é renderizado novamente

1. Quanto o estado altera
2. Quando a propriedade altera
3. Quando um componente pai renderiza novamente

a key entende o que já ta em tela e o que nao tava

## Por que não posso usar o índice do array?

A informação precisa ser fixa.

imutabilidade -> as variáveis não sofrem mutação, nós criamos um novo valor (um novo espaço na memória)

## Closures

Sempre que for atualizar uma informação, e essa informação depende do valor que ela tinha anteriormente
pode utilizar desse padrão de funções, exemplo:
function handleLikeComment(){
setLikeCount((state) => {
return state + 1
})

setLikeCount((state) => {
return state + 1
})
}

## Questões

- Das seguintes alternativas, qual é a maneira correta de se usar o map para iterar um array e exibir o valor do item em tela? Considere o array sendo um array de strings, como [’item1’, ‘item2’, ‘item3’].

array.map(item => <p>{item</p>})

- Qual a forma correta de se adicionar um valor que existe na variável novoItem ao final de um array em um estado chamado items no React?

setItems(state => [...state, novoItem])

#######
