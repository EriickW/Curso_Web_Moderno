# CSS

## Flexbox

- [Pasta do FlexBox](./FlexBox)

### ***Terminologia***
- Flex container
    - Flex item
- Nesting (conceito de que elementos vivem dentro de outro elemento)
- Axis (é a ideia de eixo )
    - main (Horizontal)
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
- [Pasta do FlexBox](./FlexBox/flex-wrap)
*flex-wrap* (Capacidade que o flex tem de usar multi linas)
- Podemos usar multi linhas 
- Cada nova linha, um novo felx container
- Exemplo: Se os itens não couberem mais na div por exemplo, a div tem `width:100px` e tem quatro itens cada um com `width:50px` usando o `flex-wrap` você avisa ao flex que quando os itens nao caberem mais no container é para quebrar linha

***flex-flow***
- shorthand
- flex-direction || flex-wrap
- Uma abreviação escrita assim `flex-flow: column wrap`
- Na abreviação vem primeiro o flex-direction depois o wrap

***Alinhamento***

*Eixo Principal (Horizontal)*

`justify-content`
- [Pasta do justify-content ](./FlexBox/justify-content)
 - Alinhamento dos elementos dentro do container 
 - Distribuiçao dos elementos

- *Valores*
    - flex-start (Alinha todos os itens do container horizontalmente no começo)
    - flex-end (Alinha todos os itens do container horizontalmente no fim)
    - center (Alinha todos os itens do container horizontalmente no começo)
    - space-around (Cria espaço ao redor dos elementos)
    - space-between (Cria espaço ao entre dos elementos)
    - space-evenly (Cria espaço ao por igual dos elementos ou seja o espaçamento será igual para todos os itens)

*Eixo Cruzado*

`align-items`
- [Pasta do justify-content ](./FlexBox/justify-content)
- Alinhamento dos elementos no eixo cruzado

*Valores*
- stretch(Padrão)
- flex-start (Deixaria eles alinahdos no começo do eixo vertical )
- flex-end (Deixaria eles alinahdos no fim do eixo vertical )
- center (Deixaria eles alinahdos no centro do eixo vertical )


**Espaços entre os itens**

`gap`
- [Pasta do justify-content ](./FlexBox/gap)
- Espaços entre os elementos 

*valores*
- Unidade de medidas 
- fixas: px, pt
- flexíveis: %, em, rem


<hr>

## Propriedades para os itens
**flex-basis**
- Define o tamanho inicial dos elementos, em unidades de pixel, antes que o espaço remanescente seja redistribuído. O valor inicial desta propriedade é auto — neste caso o navegador observa se os itens possuem o mesmo tamanho.
**flex-grow**
- [Pasta do justify-content ](./FlexBox/flex-grow)
- O crescimento do item dentro do container em relação aos espaços vazios
- Faz com que o item com o atributo ocupe frações de espaço
**flex-shrink**
- [Pasta do justify-content ](./FlexBox/flex-shrink)
- A capacidade do item encolher dentro do container
**flex**
- shorthand
- flex-grow flex-shrink flex-basis
- podem ter 1,2 e 3 valores
**order**