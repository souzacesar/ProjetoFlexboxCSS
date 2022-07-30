Posicionando Elementos com FlexBox e CSS

1 - Introdução ao Flexbox
2 - Fundamentos do Flexbox
3 - Projeto Navegador

Flex Container
Propriedades relacionadas

- Display /* Iniciador do container
- flex-direction /* Vai fazer o direcionamento seja em linha ou seja em coluna
- flex-wrap /* Que vai se aplicar para quebra de linha ou não
- flex-flow /* Que é uma abreviação pro direction e wrap
- justify-content /* Vai linhar os item do container de acordo com a sua direção
- align-items /* vai alinhar seu itens de acordo com o seu eixo
- aligin-content /* vao alinhar as linhas desse container

 Flex Item
 são os elementos filhos diretos do Flex Container. E também podem se tornar Flex Container.

 Flex Item
 Propriedades relacionadas

- Flex-grow /* definir o fator de crescimento
- flex-basis /* definir o tamanho inical desse item antes da distribuição do espaço restante dentro do container
- flex-shrink /* define a capacidade de redução
- flex /* é uma abreviação das 3 propriedades flex-shrink,flex-basis e flex-grow
- order /* relacionado a ordem de distribuição e listagem desses itens
- align-self /* vai definir o alinhamento de um item especifico desse nosso container

  Flex-direction

É a propriedade que estabelece o eixo principal do container, definindo assim a direção que os flex itens são colocados no flex-container.
São basicamente 2 eixos linha (horizontal) e coluna(vertical)

Os eixos

- row (padrão): á direção do texto, esquerda para direita
- row reverse: sentido oposto á direção do texto
- column: ordenação de cima para baixo, em coluna unica
- column-reverse: ordenação inversa, de baixo para cima

  Flex wrap
  É a propriedade que define s os itens devem ou não quebrar a linha.
  por padrão eles não quebram linhas, isso faz com que os flex itens sejam compactados além do conteúdo.

  nowrap

- nowrap: é o padrão, não permite a quebra de linha.

  wrap

- wrap: permite a quebra de linha assim que um dos flex itens não puder mais ser compactados.

  wrap-reverse
  wrap: permite a quebra de linha assim que um dos flex itens não puder mais ser compactados, porém na direção contrária da linha, acima.

FLEX-FLOW
É un atalho para as propriedades flex-direction e flex-wrap
Porém seu uso não é tão comum, visto que, quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap

JUSTIFY CONTENT
Essa propriedade vai se encarregar de alinhar os itens dentro do container de acordo com a direção e tratar da distribuição de espaçamentos entre eles

OBS: caso seus itens esteja ocupando 100% de todo o container, ela não se aplica.

As variações

- flex-start: inicio do container
- flex-end: final do container
- center: ao centro do container
- space-between:cria um espaçamento igual entre os elementos.
- space around: os espaçamentos do meio são duas vezes maiores que o inicial final

Estrutura Basica e prática com align itens

Align itens

Trata do alinhamento dos flex itens de acordo com o eixo do container.

O alinhamento é diferente para quando os itens estão com colunas ou linhas.

Permite o alinhamento central no eixo vertical.

Tipos de Alinhamento
*center: alinhamento dos itens ao centro

*stretch: padrão, e os flex itens cresçam igualmente.

*flex-start alinhamento dos itens no inicio.

*flex-end: alinhamento dos itens no final

*baseline: alinhamento de acordo com a linha base da tipografia dos itens.

Align-content

É a propriedade responsável por tratar das linhas do container em ralação ao eixo vertical do container.
Precisamos que:

 *O container utilize quebra de linhas.
 *A altura do container seja maior que a soma das linhas dos itens.

Tipos de alinhamentos

*Center: alinhamento dos itens ao centro
*stretch: é o padrão e os flex itens crescem igualmente.
*flex-start: alinhamento dos itens no início
*flex-end: alinhamento dos itens no final.
*/space-between: cria um espaçamento igual entre os elementos.
*/space-around: os espaçamentos do meio são duas vezes maior que o inicial e final.

Flex-grow

Define a proporcionalidade de crescimento dos itensn respeitando o tamanho de seus conteúdos internos.
OBS: não irá funcionar caso tenhamos adicionado justify-content ao nosso flex container.

Flex-basis

É a propriedade que estabelece o tamanho inicial do item antes das distribuição de espaço dentro dele, usando como base interno disposto.

Valores possíveis

*auto:caso o item não tenha tamanho, este será proporcional ao conteúdo do item.
*px,%¨, em, ...: são valores exatos previamente definidos
*0(zero):terá relação com a definição do flex-

Flex-shrink
É a propriedade que estabelece a capacidade de redução ou compressão do tamanho de um item.

Estrutura básica e prática Order
esta propriedade lida diretamente com a ordenação dos itens

Estrutura básica e prática com align-self
É a propriedade que estabelece o alinhamento de modo individual sobre um determinado item.

Valores possíveis

- auto: valor padrão, irá respeitar a definição de align-items do container
- flex-start: ao inicio do container
- flex-end: ao final do container
- center: relativo ao centro de acordo com o eixo
- stretch: ocupa todo os espaço relativo
- baseline: utiliza a linha base da tipografia
