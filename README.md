# www.petmatematica.ufpr.br

Esse é o repositorio oficial do site PET Matemática da UFPR. O site é escrito em [Hugo](https://gohugo.io/) com o tema [Blowfish](https://blowfish.page/).

## Pré-requisitos

Para iniciar o desenvolvimento, é necessário:

- [Node](https://nodejs.org/en/download/package-manager) v20.18.0 (LTS);
- [Hugo](https://github.com/gohugoio/hugo#installation) latest;
- [Github Desktop](https://desktop.github.com/download/) (recomendado) ou [Git](https://git-scm.com/downloads);
- um editor de texto como [VS Code](https://code.visualstudio.com/) (recomendado).

Clone o repositório localmente, usando a ferramenta [Github Desktop](https://docs.github.com/en/desktop/adding-and-cloning-repositories/cloning-a-repository-from-github-to-github-desktop) (recomendado) ou pelo `git` usando:

```
$ git clone https://github.com/PET-Matematica-UFPR/petmatematica.ufpr.br.git
```

Para baixar o Hugo, vá em [Releases](https://github.com/gohugoio/hugo/releases), clique em `Show all 24 assets` e baixe a versão `extended` para o seu sistema. Descompacte o executável `hugo` na raíz do repositório.

Em particular no sistema `windows-amd64` (se você não sabe o seu sistema, muito provavelmente é esse), o arquivo se chama `hugo_extended_x.xxx.x_windows-amd64.zip`.

## Desenvolvimento

Para instalar as dependências, você precisa rodar estes comandos na pasta do repositório:
- `git submodule update --init --recursive`. Esse clona os submódulos, tipo o tema Blwofish.
- `npm install`. Responsável por fazer download das dependência do nosso repositório.
- `npm --prefix themes/blowfish/ install`. Responsável por fazer download das dependência do tema.

Não é uma boa prática guardar imagens e arquivos grandes no repositório, dito isso, esses arquivos estão sendo guardados no Google Drive divulgacao.petmatufpr@gmail.com. Então é preciso baixar os arquivos do Drive e descompata-los na pasta `assets/arquivos`. Qualquer atualização de imagem deve ser feita no Google Drive também. É um sistema péssimo, estou pensando em outra forma.

E para iniciar o servidor de desenvolvimento use `npm run dev`. No seu navegador, acesse `localhost:1313`, toda mudança será automaticamente atualizada nesse site.

Se estiver usando o VS Code, é recomendado o uso do [terminal integrado](https://code.visualstudio.com/docs/terminal/basics) para rodar esses comandos.

## Documentação

As documentação do [Hugo](https://gohugo.io/documentation/), [Blowfish](https://blowfish.page/docs/), [TW Elements](https://tw-elements.com/docs/standard/getting-started/quick-start/) e [Tailwind CSS](https://tailwindcss.com/docs/utility-first) são essenciais.

### Tailwind CSS

O Tailwind css é uma biblioteca de estilos, ela nos da uma infinidade de classes. Vamos evitar escrever css's e usar apenas as classes dela. Por exemplo, para mudar a cor do texto e a cor de fundo basta escrever:

```html
<p class="text-blue-600 bg-red-800">
  Esse texto é azul com a cor de fundo vermelha.
</p>
```

Há muita, muitas mesmos, classes para usar, vide a [documentação](https://tailwindcss.com/docs/utility-first).

### Hugo

É o nosso framework, todo o site é construido nele. É um gerador de site estático, escrevemos conteúdo e ele compila em arquivos `.html` para subir pro servidor. Os arquivos na pasta `content/` devem ser do formato `.md` ou `.html` e são o conteúdo das nossas páginas. Por exemplo, o conteúdo da página `/sobre` está todo em `content/sobre.md`.

### Blowfish

É o tema que usamos, ele faz a maior parte do trabalho por nós. Ele deixa as páginas bonitinhas, e, quando queremos mudar, basta sobrescrever os arquivos em `layout/`. Também nos da [inúmeros shortcodes](https://blowfish.page/docs/shortcodes/) pra por no site.
