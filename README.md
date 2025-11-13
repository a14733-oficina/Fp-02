# Total 90 - Catálogo de Camisolas de Futebol

## Descrição do Projeto

O projeto **Total 90** é um website estático que simula um catálogo de venda de camisolas de futebol de clubes e seleções internacionais. O objetivo principal é apresentar uma seleção de artigos e fornecer informações sobre a equipa e contactos.

O website utiliza uma estrutura simples e focada em design responsivo para garantir uma visualização adequada em diferentes dispositivos.

## Funcionalidades Principais

*   **Página Inicial (`index.html`):** Apresenta a marca "Total 90", uma breve descrição e artigos de destaque.
*   **Catálogo de Produtos (`catalogo.html`):** Exibe uma lista de camisolas disponíveis com imagens e botões de "Comprar" (que redirecionam para páginas de detalhe como `PORTO.html`, `inter.html`, `boca.html`).
*   **Página da Equipa (`Equipa.html`):** Apresenta os membros da equipa com as respetivas funções e fotografias.
*   **Página de Contacto (`contacto.html`):** Destina-se a fornecer informações de contacto (o conteúdo desta página não foi detalhado, mas a navegação existe).
*   **Design Responsivo:** O layout adapta-se a telemóveis, tablets e desktops através de media queries.

## Estrutura de Ficheiros

O projeto segue uma estrutura de diretórios padrão para um website estático:

```
/
├── boca.html
├── catalogo.html
├── contacto.html
├── Equipa.html
├── index.html
├── inter.html
├── PORTO.html
├── audio/
├── css/
│   └── style.css
├── images/
│   ├── BOCA.webp
│   ├── PORTO.webp
│   ├── inter.webp
│   ├── atletico.webp
│   ├── Mexico.webp
│   └── (outras imagens de perfil)
├── js/
│   └── script.js (vazio)
└── media/
```

## Detalhes do Código HTML e CSS

O website é construído com base em HTML5 e CSS, com foco em layout flexível:

*   **Estrutura HTML:**
    *   Todas as páginas compartilham uma estrutura básica com um cabeçalho (`<header>`) que contém o título da marca (`Total 90`) e a barra de navegação (`<nav>`).
    *   O conteúdo principal é envolvido pela *tag* `<main>`, com secções como `hero` (destaque) e `servicos` (catálogo/equipa).
    *   O rodapé (`<footer>`) é consistente em todas as páginas.
*   **Estilização (CSS):**
    *   O CSS está **incorporado** na *tag* `<style>` dentro de cada ficheiro HTML, o que é uma prática que pode dificultar a manutenção.
    *   Utiliza a fonte 'Inter', sans-serif.
    *   As cores predominantes são o azul (`#0d6efd`) para o cabeçalho e botões, e tons escuros para o rodapé (`#343a40`).
    *   **Layout Grid:** A secção `.servicos` utiliza **CSS Grid** para criar layouts de catálogo e equipa, ajustando o número de colunas consoante o tamanho do ecrã.
    *   **Responsividade:** O design é adaptado para três pontos de interrupção (breakpoints):
        *   **Dispositivos Móveis (Padrão):** Layout de uma coluna.
        *   **Tablets (`min-width: 768px`):** Layout de duas colunas.
        *   **Desktops (`min-width: 1024px`):** Layout de três colunas e navegação horizontal no cabeçalho.
