# CSS

## Flexbox

- [Pasta do FlexBox](./FlexBox)

### ***Terminologia***
- Flex container
    - Flex item
- Nesting (conceito de que elementos vivem dentro de outro elemento)
- Axis (é a ideia de eixo )
    - main
        - start, end
    - cross (cruzado)
        - start, end
- Flex sizing
    - flexível
    - altera width/height dois itens para preenchimento dos espaços do flex container (usando a proprieda de css flex:1 nos items você faz com que aja uma alteração de tamanho para que eles preenchão todo o container)

### ***Propiedades do flex Container***

**Direção dos itens**
- Flex é uma dimensão (horizontal ou vertical)
- podemos mudar a direção com `flex-direction`
- valores: (row | row-reverse | column | column-reverse)
- o valor padrão do flex-direction é o row (que no caso seria em linha), e o row-reverse ele meio que inverte a posição em linha 
- O valor column muda o eixo do flex fazendo todos os itens ficarem em posição vertical ou seja em coluna 

**Multi linhas** 
*flex-wrap* (Capacidade que o flex tem de usar multi linas )
- Podemos usar multi linhas 
- Cada nova linha, um novo felx container



**Alinhamento**
    - Principal 
    - Cruzado 
**Espaços entre os itens**