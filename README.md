# Projeto Social

Página web interativa que simula a tela de um smartphone para apresentar atalhos de redes sociais. Ao selecionar um dos ícones laterais, a página correspondente é carregada dentro da moldura do celular por meio de um `iframe`.

O projeto foi desenvolvido como atividade prática a partir das aulas do professor **Gustavo Guanabara**, do [Curso em Vídeo](https://www.youtube.com/@cursoemvideo), com foco em HTML5, CSS3, posicionamento de elementos e incorporação de páginas.

## Funcionalidades

- Exibição de uma interface inspirada em um smartphone;
- Navegação entre telas de redes sociais por meio de ícones;
- Carregamento das telas internas dentro de um `iframe`;
- Botão **Acesse** em cada tela, que abre o perfil correspondente em uma nova aba;
- Efeito visual nos ícones ao passar o cursor;
- Layout centralizado sobre uma imagem de fundo;
- Organização das telas internas em uma pasta própria (`telas/`).

## Redes sociais disponíveis

A interface possui atalhos para:

| Atalho    | Tela                  | Destino do botão **Acesse**                                         |
|-----------|-----------------------|---------------------------------------------------------------------|
| Home      | `telas/home.html`     | — (tela inicial, sem botão)                                         |
| YouTube   | `telas/youtube.html`  | [Curso em Vídeo](https://www.youtube.com/@cursoemvideo)             |
| GitHub    | `telas/github.html`   | [gustavoguanabara](https://github.com/gustavoguanabara)             |
| Instagram | `telas/instagram.html`| [@gustavoguanabara](https://www.instagram.com/gustavoguanabara/)    |
| Twitter/X | `telas/twitter.html`  | [@guanabara](https://x.com/guanabara)                               |
| Facebook  | `telas/facebook.html` | [gustavoguanabara](https://www.facebook.com/gustavoguanabara)       |

Todos os links apontam para os perfis do professor Gustavo Guanabara / Curso em Vídeo, mantendo as referências utilizadas no material didático original (veja [Referências](#referências)).

## Como funciona

A página `index.html` é a tela principal. Ela apresenta:

1. Uma moldura de celular criada com a imagem `imagens/frame-iphone.png`;
2. Um `iframe` chamado `tela`, que exibe a tela inicial (`telas/home.html`);
3. Ícones laterais para cada rede social;
4. Links com o atributo `target="tela"`, que fazem o conteúdo abrir dentro do `iframe`.

Cada tela interna (exceto a Home) possui uma imagem relacionada à rede social e um botão **Acesse**, que abre o endereço correspondente em uma nova aba (`target="_blank"`).

## Tecnologias utilizadas

- **HTML5** para a estrutura das páginas;
- **CSS3** para posicionamento, cores, fundo, sombras e efeitos de interação;
- **`iframe`** para carregar as telas sociais dentro da moldura do celular;
- Imagens locais para representar o aparelho, os ícones e as telas das redes sociais.

O projeto é totalmente estático e pode ser publicado no **GitHub Pages** ou em qualquer outro servidor de arquivos estáticos.

## Estrutura do projeto

```text
Projeto_Social/
├── index.html
├── telas/
│   ├── home.html
│   ├── youtube.html
│   ├── github.html
│   ├── instagram.html
│   ├── twitter.html
│   └── facebook.html
├── estilos/
│   ├── style.css
│   └── social.css
├── imagens/
│   ├── favicon.ico
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
│   ├── tela-instagram.jpg
│   ├── tela-twitter.jpg
│   ├── tela-facebook.jpg
│   ├── foto-gitHub.jpg
│   ├── foto-instagram.jpg
│   ├── foto-twiter.jpg
│   └── foto-facebook.jpg
├── .gitattributes
├── LICENSE
└── README.md
```

### Principais arquivos

- `index.html`: página principal com a moldura do celular, o `iframe` e os atalhos sociais;
- `telas/home.html`: tela inicial exibida dentro do aparelho (estilo próprio, embutido no arquivo);
- `telas/*.html`: telas das redes sociais carregadas no `iframe`;
- `estilos/style.css`: estilos da página principal, incluindo o fundo, o telefone, o `iframe` e os ícones;
- `estilos/social.css`: estilos compartilhados pelas telas das redes sociais (imagem em largura total e botão **Acesse**);
- `imagens/`: recursos visuais usados na interface, incluindo o `favicon.ico`.

## Como executar localmente

O projeto é estático e não possui dependências nem processo de compilação.

```bash
git clone https://github.com/RafaelRodriguesMagdaleno/Projeto_Social.git
cd Projeto_Social
```

### Opção 1: abrir diretamente no navegador

Abra o arquivo `index.html` no navegador.

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
- Uso de links com `target` para controlar o destino do conteúdo (`iframe` nomeado e nova aba);
- Incorporação de documentos com `iframe`;
- Caminhos relativos entre pastas (`../estilos/`, `../imagens/`);
- Posicionamento absoluto com `position: absolute`;
- Centralização com `top: 50%`, `left: 50%` e `transform: translate(-50%, -50%)`;
- Aplicação de imagens de fundo com `background-image` e `background-attachment: fixed`;
- Ajuste de imagens com `background-size: cover`;
- Criação de efeitos de hover com CSS e transições;
- Uso de sombras, bordas arredondadas e ocultação da barra de rolagem;
- Organização de páginas, estilos e imagens em diretórios separados.

## Referências

Os links das telas sociais permanecem direcionados aos perfis do professor Gustavo Guanabara e do Curso em Vídeo. Essa escolha foi mantida porque o projeto foi desenvolvido a partir do conteúdo ensinado por ele, e funciona também como crédito ao material utilizado para aprender a construir o projeto.

## Créditos

Projeto desenvolvido por [Rafael Rodrigues Magdaleno](https://github.com/RafaelRodriguesMagdaleno) a partir das aulas do professor [Gustavo Guanabara](https://www.youtube.com/@cursoemvideo), do Curso em Vídeo.

O projeto possui finalidade educacional.

## Licença

Distribuído sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
