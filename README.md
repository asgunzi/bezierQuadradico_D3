
# Curva de Bezier quadrática - escrita em JS D3


## Curva de Bézier interativa

A curva de Bézier é uma curva bastante elegante, formada a partir de um número de retas e com aplicações surpreendentes.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bezier01.jpeg)

Ela foi criada pelo francês Pierre Bézier, funcionário da Renault, nos anos 1960 – chama a atenção também a data, relativamente muito recente para uma construção matemática simples.

Fiz uma versão interativa em Javascript D3, para mexer e sentir como ela funciona, disponível em:

[https://asgunzi.neocities.org/ArteMatematica/Bezier01](https://asgunzi.neocities.org/ArteMatematica/Bezier01)

Alguns prints abaixo:

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bezier02.jpeg)

Basta arrastar qualquer dos pontos que formam as retas, para criar uma nova curva.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bezier03.jpeg)

## Como traçar a curva?

Vou explicar aqui a curva quadrática.

Pegue duas retas e divida em p pedaços.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bez_constr01.png)

Una o p-ésimo pedaço do primeiro com o p-ésimo pedaço do segundo (do final para o começo), usando uma reta.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bez_constr02.png)


Divida essa última reta em p pedaços também, e marque o p-ésimo pedaço.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bez_constr04.png)


Repita o procedimento até o fim, e teremos a nossa curva.

![](https://ideiasesquecidas.files.wordpress.com/2023/07/bez_constr05.png)


No caso com duas retas, teremos uma curva quadrática. É possível fazer procedimento similar com mais retas – se forem três, teremos uma cúbica, por exemplo.


## E para que serve?
Bézier desenvolveu a curva para auxiliar o design de carros da Renault, a fim de tornar as curvas mais elegantes. Ou seja, dá para dizer que, desde Bézier, a curva ajuda a fazer o projeto de carros da Renault.


![](https://ideiasesquecidas.files.wordpress.com/2023/07/cdarro.png)

Foto da fonte a seguir.

https://www.bricsys.com/pt-br/blog/the-bezier-curve-how-car-design-influenced-cad

A técnica da curva de Bézier foi incorporada em sistemas CAD diversos, por ser uma curva suave contida no “convex hull” das retas, ou seja, no contorno de uma área dada pelas retas.

Nada mau para uma construção matemática simples!

Próximas rotinas a serem feitas são a curva de Bézier cúbica e de ordens superiores. Estão na lista de tarefas!

A rotina foi feita em parceria com o amigo Ernée Kozyreff Filho.
