--------------------------------------------------

* DISPLAY: FLEX; 

- Por padrão o **display: flex;** sempre alinha os itens horizontalmente

--------------------------------------------------

* FLEX-DIRECTION: 

- flex-direction por padrão tem o valor "row" (linha):
{
 -  **flex-direction: row;** // Alinha itens horizontalmente (ou em linha) da esquerda para direita
 
 - **flex-direction: column;** // Alinha itens em coluna de cima para baixo

 - **flex-direction: row-reverse;** // Alinha itens horizontalmente da direita para esquerda

 - **flex-direction: row-column;** // Alinha itens em coluna de baixo para cima
}

--------------------------------------------------

* ALIGN-ITEMS e JUSTIFY-CONTENT

* ALIGN-ITEMS [ - serve para alinhar verticalmente - ]
 - **flex-start;** -> serve para alinhar no começo 
 - **flex-end;** -> serve para alinhar no final
 - **center;** -> serve para alinhar itens no meio

* JUSTIFY-CONTENT [ - serve para alinhar horizontalmente - ]
 - **flex-start;** -> serve para alinhar no começo
 - **flex-end;** -> serve para alinhar no final
 - **center;** -> serve para alinhar itens no meio
 - **space-between;** -> serve para colocar um mesmo espaço entre os itens selecionados na página
 - **space-around;** -> serve para colocar um mesmo espaço em volta dos itens selecionados na página

Exemplo de utilização de ALIGN-ITEMS junto com JUSTIFY-CONTENT:

// Centralizando no meio da página
classe_ou_id {
  // flex-direction: column;

  **aling-items: center;**
  **flex-direction: center;**
}

--------------------------------------------------

* FLEX-GROW, FLEX-SHRINK e FLEX

 - **flex-grow: 1;** -> Aqui estamos dizendo que o componente (ou item) aceita ser aumentado com base no elemento pai (container)

 - **flex-shrink: 1;** -> Aqui estamos dizendo que o componente (ou item) aceita ser espremido para caber no elemento pai (container)

 - **flex: 1 0;** [- Parâmetros > flex: <flex-grow>, <flex-shrink> -] -> Aqui estamos dizendo que o componente (ou item) aceita ser aumentado com base no elemento pai (container) e não aceita ser espremido.

--------------------------------------------------

* FLEX-WRAP e ALIGN-CONTENT


* FLEX-WRAP

 - **flex-wrap: wrap;** -> Mantêm o tamanho do elemento e realiza quebra de linha
 - **flex-wrap: wrap-reverse;** -> Mantêm o tamanho do elemento e realiza quebra de linha, os elesmentos começam do final da página

* ALIGN-CONTENT

 - **align-content: [ tem as mesmas funcionalidades do "justify-content" ];** -> serve para alinhar os elementos quanto há mais de uma linha quebrada

 --------------------------------------------------

 * ORDER

 - O "**order**" serve para ordenação de componentes em tela. No exemplo abaixo estamos ordenando como primeiro item **.blue**, em seguida **.red** e por fim **.green**

                                .red {
                                  background: #f00;
                                  order: 1;
                                }

                                .green {
                                  background: #0f0;
                                  order: 2;
                                }

                                .blue {
                                  background: #00f;
                                  order: 0;
                                }

--------------------------------------------------