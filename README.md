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

