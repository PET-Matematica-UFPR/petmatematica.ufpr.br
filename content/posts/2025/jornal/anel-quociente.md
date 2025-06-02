+++
title = "Um anel quociente conveniente"
date = 2025-06-01T08:00:00-03:00
draft = false

tags = ["petiscos"]
eventos = []
+++

{{< katex >}}

Um anel é um conjunto \\(A\\) munido de duas operação: \\(+: A \times A \to A\\) e \\(\cdot: A \times A \to A\\) chamadas de adição e produto, respectivamente, tais que:

- (S1) \\((a+b)+c = a+(b+c)\\) para todo \\(a,b,c \in A\\) (associtividade da soma);
- (S2) Existe \\(0 \in A\\) tal que \\(a+0 = a = 0+a\\), para todo \\(a \in A\\) (elemento neutro da soma);
- (S3) Para cada \\(a \in A\\) existe um elemento \\(b \in A\\) tal que \\(a+b = b+a = 0\\) (oposto da soma);
- (S4) \\(a+b = b+a\\), para todo \\(a,b \in A\\) (comutativade da soma);
- (P1) \\(a \cdot (b \cdot c) = (a \cdot b) \cdot c\\), para todo \\(a,b,c \in A\\) (associativade do produto);
- (D) \\(a \cdot (b+c) = a \cdot b + a \cdot c\\) e \\((a+b) \cdot c = a \cdot c + b \cdot c\\), para todo \\(a,b,c \in A) (distributividade).

Considere o corpo \\(\R \\) munido das operações de soma \\(+ \\) e produto \\(\cdot \\) usuais. \\(\R[x] \\) é o anel de polinômios com coeficientes em \\(\R \\). Um elemento qualquer \\(p(x) \in \R[x] \\) é da forma:

$$
p(x) = a_0 + a_1 \cdot x + ... + a_n \cdot x^n =\sum_{i=0}^n a_i \cdot x^i \text{,}
$$

onde \\(a_i \in \R \\) para todo \\(i=1,2,...,n \\), \\(a_n \neq 0 \\) e para algum \\(n \in \N \\).

Como \\(\R \\) é um corpo, o anel de polinômios correspondente é uma domínio de ideias principais, isto é, para todo ideal \\(I \\) de \\(\R[x] \\) existe um elemento \\(f(x) \in \R[x]\\) tal que \\(I \\) é gerado por \\(f(x) \\) .
