# Projeto Social

Página web interativa que simula a tela de um smartphone para apresentar atalhos de redes sociais. Ao selecionar um dos ícones laterais, a página correspondente é carregada dentro da moldura do celular por meio de um `iframe`.

O projeto foi desenvolvido como atividade prática a partir das aulas do professor **Gustavo Guanabara**, do [Curso em Vídeo](https://www.youtube.com/@cursoemvideo), com foco em HTML5, CSS3, posicionamento de elementos e incorporação de páginas.

## Funcionalidades

- Exibição de uma interface inspirada em um smartphone;
- Navegação entre páginas de redes sociais por meio de ícones;
- Carregamento das páginas internas dentro de um `iframe`;
- Links para os perfis correspondentes em uma nova aba;
- Efeito visual nos ícones ao passar o cursor;
- Layout centralizado sobre uma imagem de fundo;
- Organização das páginas sociais em uma pasta própria.

## Redes sociais disponíveis

A interface possui atalhos para:

- Home;
- YouTube;
- GitHub;
- Instagram;
- Twitter;
- Facebook.

A página do GitHub direciona para o perfil de [Rafael Rodrigues Magdaleno](https://github.com/RafaelRodriguesMagdaleno). A página do YouTube direciona para o canal do [Curso em Vídeo](https://www.youtube.com/@cursoemvideo), mantendo a referência utilizada no material didático original.

## Como funciona

A página `index.html` é a tela principal. Ela apresenta:

1. Uma moldura de celular criada com a imagem `frame-iphone.png`;
2. Um `iframe` que inicia carregando `home.html`;
3. Ícones laterais para cada rede social;
4. Links com o atributo `target="tela"`, que fazem o conteúdo abrir dentro do `iframe`.

Cada página interna possui uma imagem relacionada à rede social e um botão **ACESSE**, que abre o endereço correspondente em uma nova aba.

## Tecnologias utilizadas

- **HTML5** para a estrutura das páginas;
- **CSS3** para posicionamento, cores, fundo, sombras e efeitos de interação;
- **`iframe`** para carregar as páginas sociais dentro da moldura do celular;
- **GitHub Pages** ou outro servidor estático para publicação;
- Imagens locais para representar o aparelho, os ícones e as telas das redes sociais.

## Estrutura do projeto

```text
Projeto_Social/
├── index.html
├── home.html
├── favicon.ico
├── estilos/
│   ├── social.css
│   └── style.css
├── imagens/
│   ├── fundo-madeira.jpg
│   ├── frame-iphone.png
│   ├── logo-home.jpg
│   ├── logo-youtube.jpg
│   ├── logo-github.jpg
│   ├── logo-instagram.jpg
│   ├── logo-twitter.jpg
│   ├── logo-facebook.jpg
│   ├── tela-home.jpg
│   ├── tela-youtube.png
│   ├── tela-github.jpg
│   ├── foto-gitHub.jpg
│   ├── foto-instagram.jpg
│   ├── foto-twiter.jpg
│   └── foto-facebook.jpg
├── paginas-sociais/
│   ├── youtube.html
│   ├── github.html
│   ├── instagram.html
│   ├── twitter.html
│   └── facebook.html
└── LICENSE
```

### Principais arquivos

- `index.html`: página principal com a moldura do celular, o `iframe` e os atalhos sociais;
- `home.html`: tela inicial exibida dentro do aparelho;
- `estilos/style.css`: estilos da página principal, incluindo o fundo, o telefone e os ícones;
- `estilos/social.css`: estilos compartilhados pelas páginas internas das redes sociais;
- `paginas-sociais/`: páginas carregadas no `iframe`;
- `imagens/`: recursos visuais usados na interface;
- `favicon.ico`: ícone do site.

## Como executar localmente

O projeto é estático e não possui dependências ou processo de compilação.

### Opção 1: abrir diretamente no navegador

Baixe ou clone o repositório e abra o arquivo `index.html` no navegador.

### Opção 2: utilizar um servidor local

Para evitar limitações de alguns navegadores ao trabalhar com arquivos locais, utilize uma extensão como **Live Server** no Visual Studio Code ou um servidor HTTP local.

Com Python instalado, também é possível executar:

```bash
python3 -m http.server 8000
```

Depois, acesse:

```text
http://localhost:8000
```

## Conceitos praticados

O projeto exercita conceitos importantes de desenvolvimento front-end, como:

- Estruturação de páginas com HTML5;
- Uso de links com `target` para controlar o destino do conteúdo;
- Incorporação de documentos com `iframe`;
- Posicionamento absoluto com `position: absolute`;
- Centralização com `transform: translate`;
- Aplicação de imagens de fundo com `background-image`;
- Ajuste de imagens com `background-size: cover`;
- Criação de efeitos de hover com CSS;
- Uso de sombras, bordas arredondadas e transições;
- Organização de páginas, estilos e imagens em diretórios separados.

## Referência do YouTube

A página do YouTube permanece direcionada ao canal do Curso em Vídeo. Essa escolha foi mantida porque o projeto foi desenvolvido a partir do conteúdo ensinado pelo professor Gustavo Guanabara

Essa referência também funciona como crédito ao material utilizado para aprender a construir o projeto.

## Créditos

Projeto desenvolvido por [Rafael Rodrigues Magdaleno](https://github.com/RafaelRodriguesMagdaleno) a partir das aulas do professor [Gustavo Guanabara](https://www.youtube.com/@cursoemvideo), do Curso em Vídeo.

O projeto possui finalidade educacional.
