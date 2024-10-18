# www.petmatematica.ufpr.br

Esse é o repositorio oficial do site PET Matemática da UFPR. O site é escrito em [Hugo](https://gohugo.io/) com o tema [Blowfish](https://blowfish.page/). 

## Pré-requisitos

Para iniciar o desenvolvimento, as seguintes dependências são necessárias:

- [Node](https://nodejs.org/en/download/package-manager) v20.18.0 (LTS);
- [Hugo](https://github.com/gohugoio/hugo#installation) latest.

Caso tenha problema em instalar alguma, peça ajuda!

## Documentação

As documentação do [Hugo](https://gohugo.io/documentation/), [Blowfish](https://blowfish.page/docs/), [TW Elements](https://tw-elements.com/docs/standard/getting-started/quick-start/) e [Tailwind css](https://tailwindcss.com/docs/utility-first) são essenciais.

### Tailwind css

O Tailwind css é uma biblioteca de estilos, ela nos da uma infinidade de classes. Vamos evitar escrever css's e usar apenas as classes dela. Por exemplo, para mudar a cor do texto e a cor de fundo basta escrever:

```html
<p class="text-blue-600 bg-red-800">Esse texto é azul com a cor de fundo vermelha.</p>
```

Há muita, muitas mesmos, classes para usar, vide a [documentação](https://tailwindcss.com/docs/utility-first).

### Hugo

É o nosso framework, todo o site é construido nele. É um gerador de site estático, escrevemos conteúdo e ele compila em arquivos html para subir pro servidor. Os arquivos na pasta `content/` devem ser do formato `.md` ou `.html` e são o conteúdo das nossas páginas. Por exemplo, o conteúdo da página `/sobre` está todo em `content/sobre.md`.

Beleza, o conteúdo das páginas fica em `content/`, mas como o Hugo converte esse conteúdo em `html`? O tema dita como o arquivo `.html` será propriamente escrito. Na pasta do tema `theme/blowfish/` em `layout/` estão essas diretivas, ou seja, lá que diz como o header, footer e tudo mais são convertidos. Note que também temos uma pasta `layout/`, tudo que está escrito nela sobrescreve as respectivas do tema. Muito raramente vamos precisar mexer nisso. Para ir mais a fundo nisso, leia a [documentação](https://gohugo.io/templates/introduction/) do Hugo.

### Blowfish

É o tema que usamos, ele faz a maior parte do trabalho por nós. Ele deixa as páginas bonitinhas, e, quando queremos mudar, basta sobrescrever os arquivos em `layout/`. Também nos da inúmeras 