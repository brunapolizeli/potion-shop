[🇺🇸 English](README.md) | [🇧🇷 Português](README.pt-BR.md)

# Potion Shop

Uma loja interativa de poções apresentada como um grimório aberto, com layout responsivo, carrinho dinâmico e fluxo de checkout.

[**Demo ao vivo — potion-shop-three.vercel.app**](https://potion-shop-three.vercel.app/)

---

## Visão Geral do Projeto

Potion Shop começou como um aplicativo simples de menu mobile, desenvolvido como parte do Scrimba Full Stack Path e baseado em um [design Figma de menu de restaurante](https://www.figma.com/design/Hdgwo69Dym9vVsxbuPbl0h/Mobile-Restaurant-Menu?node-id=0-1&t=r8jwmyHIEVtTc5cL-1), utilizado como referência inicial. Todo o HTML, CSS e JavaScript foi escrito de forma independente, do zero, conectando um array de dados em JavaScript ao DOM e mantendo estrutura, estilo e lógica bem separados.

Posteriormente, o layout foi redesenhado como um livro de feitiços aberto: uma decisão tomada para combinar melhor com o tema e que também eliminou a necessidade de rolagem ao colocar o menu e o carrinho em páginas opostas. Uma capa de livro fechada agora funciona como tela inicial, abrindo para revelar o conteúdo ao ser clicada. O layout se adapta responsivamente à largura da viewport, com uma mensagem solicitando a rotação do dispositivo em telas estreitas no modo retrato, onde o livro aberto não caberia confortavelmente.

---

## Funcionalidades

- Itens do menu (poções) renderizados dinamicamente a partir de um array de dados em JavaScript
- Cada item exibe ícone, nome, ingredientes e preço
- Funcionalidade de adicionar ao carrinho por meio de um botão "+" em cada item
- O carrinho acompanha os itens selecionados e suas quantidades, sendo renderizado dinamicamente na página direita
- Possibilidade de diminuir a quantidade ou remover itens do carrinho usando botões de menos e lixeira
- Exibição do preço total atualizado no carrinho
- Persistência do carrinho entre recarregamentos da página usando localStorage
- Modal de checkout com formulário de dados do cartão, aberto por meio do botão "Complete order" e fechado ao clicar fora dele ou no botão de fechar
- Mensagem de confirmação exibida após o pagamento, personalizada com o nome do cliente
- Mensagem para girar o dispositivo em telas estreitas no modo retrato, substituindo o layout do livro por uma orientação para uso em modo paisagem
- Layout responsivo do livro, escalando conforme a largura da viewport (`vw`/`aspect-ratio`) em vez de dimensões fixas em pixels
- Validação de inputs para nome, número do cartão e CVV, com mensagens de erro personalizadas
- Estados de foco customizados nos campos de dados do cartão, combinando com a paleta visual do app

---

## Estrutura do Projeto

```
potion-shop/
├── assets/
│   ├── buttons/
│   │   ├── add-button.png
│   │   ├── minus-button.png
│   │   └── trash-button.png
│   ├── cursors/
│   │   ├── cursor-arrow.png
│   │   └── cursor-pointer.png
│   ├── icons/
│   │   ├── bottle-health.png
│   │   ├── bottle-mana.png
│   │   ├── bottle-stamina.png
│   │   ├── coin-icon.png
│   │   └── phone-icon.png
│   ├── banner.png
│   ├── book-bg.png
│   ├── book-cover.png
│   ├── favicon.png
│   └── moon-image.png
├── data.js
├── effects.js
├── index.css
├── index.html
├── index.js
└── README.md
```

---

## Tecnologias Utilizadas

- HTML5
- CSS3
  - Flexbox
  - Animações e keyframes
  - Design responsivo (media queries, unidades de viewport)
- JavaScript (vanilla)
  - Manipulação do DOM e delegação de eventos
  - Persistência com LocalStorage

---

## Créditos

Ícones das poções criados por [Magnific - Flaticon](https://www.flaticon.com/free-icons/potion "potion icons").

As artes do banner, da lua, do livro e do favicon foram geradas com o ChatGPT. Os ícones dos botões, do telefone e da moeda foram gerados com o Claude.

---

## Licença

Este projeto está licenciado sob a [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). É livre para uso, compartilhamento e adaptação para fins não comerciais, com atribuição.
