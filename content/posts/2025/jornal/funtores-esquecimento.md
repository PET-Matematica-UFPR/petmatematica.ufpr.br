+++
title = "Amnésia Categórica: Funtores Esquecimento"
date = 2025-06-08T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []
+++

{{< katex >}}

Vimos [anteriormente](/posts/2025/jornal/categorias/) sobre como o conceito de categorias pode criar caminhos entre vários objetos matemáticos, desta vez veremos como podemos "apagar" estes caminhos, isto é, uma passagem só de ida de uma até outra coisa. 

Dentro da _Teoria de Categorias_, foi necessário estabelecer o conceito de _Funtor_ — um morfimo entre categorias — para que possamos criar os "caminhos" mencionados anteriormente, como uma forma de associar objetos distintos. Poderíamos definir um funtor como uma tripla \\((C, f, D)\\), isto é, um morfismo \\(f: C \to D\\) entre as categorias \\(C\\) e \\(D\\) que leva os objetos \\(Ob_{C}\\) em \\(Ob_{D}\\), os morfismos \\(Mor_{C}\\) em \\(Mor_{D}\\), e que preserva tanto a composição de morfismos quanto suas identidades. Exemplos clássicos de funtores são: o funtor de _Abelianização_ e o funtor _Conjunto Potência_.

O funtor _Conjunto Potência_ é uma tripla \\((Set, P, Set)\\) que associa cada conjunto \\(A \in Ob_{Set}\\) ao seu conjunto potência \\(P(A)\\), e cada função \\(f:A \to B\\) para \\(P(f): P(A) \to P(B)\\).

O funtor de _Abelianização_ é uma tripla \\((Grp, H, Ab)\\), onde \\(Grp\\) é a categoria de grupos e \\(Ab\\) a de grupos abelianos, que associa cada grupo \\(A \in Grp\\) a um grupo \\(H(A) = A/A'\\), onde \\(A'\\) é o subgrupo comutador de \\(A\\), isto é, o subgrupo gerado por elementos de \\(A\\) da forma \\(ghg^{-1}h^{-1}\\). O funtor de abelianização, essencialmente, toma um grupo e o quocienta pelo seu subgrupo comutador para que então o "transforme" num grupo comutativo.

Agora que está definido o que é um funtor e qual a ideia geral por trás, vamos discutir um pouco sobre um tipo fundamental de funtor: o _Funtor Esquecimento_. Um funtor é dito de _esquecimento_ quando ele "esquece" alguma estrutura dos seus objetos, isto é, utilizamos ele para "remover" uma estrutura pertencente a algum objeto. Vejamos por exemplo: podemos definir um funtor \\((Grp, F, Set)\\) que associa um grupo \\(G\\) ao seu _conjunto subjacente_ \\(U(G)\\), e um homomorfismo \\(f: G \to H\\) a uma função \\(F(f):U(G) \to U(H)\\), isto é, estamos "removendo" a estrutura de grupo de \\(G\\) e deixando apenas o _conjunto_ de \\(G\\), essencialmente removendo a operação da qual o grupo era munido.

Os funtores esquecimento (de fato, há mais de um) possuem como ideia central a de "esquecer" estruturas e propriedades de um objeto, poderíamos definir um funtor de \\(Rng\\) para \\(Grp\\) e "esquecer" uma das operações do anél inicial, poderíamos retirar a comutatividade de um anél \\(A \in CRng\\) apenas aplicando-o num funtor \\(F: CRng \to Rng\\).

Enfim, desta vez demos mais profundidade a _Teoria de Categorias_ utilizando os conceitos de funtores e como podemos utilizá-los para "retirar" ou _"esquecer"_ estruturas de objetos. Foi um prazer escrever-vos, seguiremos eventualmente com mais teoria de categorias e até a próxima!