+++
title = "Categorias: O elo entre as áreas da Matemática"
date = 2025-05-22T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []
+++

{{< katex >}}

A matemática, frequentemente, é dada por várias áreas de estudo, a princípio desconexas: álgebra, geometria, análise, etc. Cada uma com objetos, aplicações e interesses distintos, onde raramente há alguma interseção. No entanto, esta disjunção não reflete a realidade: a matemática é uma só.

Analisando vários objetos matemáticos, de fato podemos ver inúmeras estruturas semelhantes: anéis e espaços vetoriais, funções e homomorfismos, operações e relações. Podemos ver que é possível descrever objetos matemáticos de uma área com a linguagem de outra: o plano euclidiano nada mais é do que um espaço vetorial, por exemplo. Esta forma de descrição constrói maquinário para expandir e provar teoremas e conjecturas. 

A ideia por trás de enxergar vários objetos de maneira unificada veio pelo conceito de _Categorias_, mais amplamente na linguagem da _Teoria de Categorias_. Estes conceitos foram introduzidos e formalizados pelo americano Saunders MacLane ao longo da década de 60 e culminando na publicação de _Categories for the Working Mathematician_, a grande obra sobre categorias até o momento. O conceito de categorias é interessante para tratar da generalização de objetos matemáticos: funções e homomorfismos se tornam apenas _Morfismos_, conjuntos e grupos se tornam meros objetos de categorias enormes como _Sets_ e _Grps_ que englobam todas estas estruturas.

Mas afinal, o que é uma categoria?

Uma categoria \\(C\\) é uma quíntupla (\\(Ob\\), \\(Mor\\), \\(dom\\), \\(cod\\), \\(\circ\\)), onde: \\(Ob\\) é sua classe de objetos, isto é, os seus "elementos", \\(Mor\\) a de morfismos ("funções" entre esses "elementos"), \\(dom\\) e \\(cod\\) são "funções" que associam um morfismo a um objeto, e \\(\circ\\) é a composição de morfismos.
Além disso, precisamos de ter duas condições satisfeitas: quando a composição está bem definida, ela deve ser associativa, e existe uma identidade para cada objeto em \\(C\\)$.

Com esta definição podemos enxergar estruturas de maneira geral e concisa: grupos são apenas objetos de \\(Grps\\), anéis de \\(Rng\\) e espaços vetorias de \\(Vec\\). Poderíamos estabelecer morfismos entre estas categorias, isto é, jeitos de transformar um grupo num espaço vetorial, ou um anel em um conjunto, ou talvez até um monóide em um espaço topológico. Estes _morfismos_ de categorias são chamados de _funtores_, e são o centro de muitas teorias.

A _Teoria de Categorias_ nos permitiu unificar a matemática de maneira direta, concisa e correta, e possibilitou uma expansão de áreas como Álgebra e Topologia, assim como a fundação de novas como _Geometria Álgebrica_.