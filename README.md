# Desafio XMX — GaraHerb Landing Page

Landing page de alta conversão para o suplemento masculino **GaraHerb**, desenvolvida com HTML semântico, SCSS modular e JavaScript vanilla.

## Visão Geral

Página de vendas (VSL/Sales Page) com foco em performance e conversão, apresentando o produto em múltiplas seções estratégicas: proposta de valor, ingredientes, depoimentos, FAQ e checkout.

## Estrutura do Projeto

```
desafio-xmx/
├── index.html              # Documento principal
├── css/
│   └── style.css           # CSS compilado (gerado pelo Sass)
├── assets/
│   ├── icons/              # SVGs e ícones
│   └── images/             # Imagens do produto e depoimentos
└── src/
    ├── js/
    │   └── script.js       # Scripts da página (accordion FAQ, etc.)
    └── scss/
        ├── style.scss      # Entry point — importa todos os partials
        ├── _variables.scss # Tokens de design (cores, tipografia, espaçamentos)
        ├── _mixins.scss    # Mixins reutilizáveis (badge-bar, card-separator)
        ├── _base.scss      # Reset e estilos globais
        ├── _components.scss# Componentes compartilhados (.btn, .fire-badge)
        ├── _hero.scss      # Seção hero
        ├── _pricing.scss   # Seção de preços / planos
        ├── _formula.scss   # Seção da fórmula
        ├── _ingredients.scss # Seção de ingredientes
        ├── _about.scss     # Seção de oferta exclusiva
        ├── _testimonials.scss # Seção de depoimentos
        ├── _shipping-banner.scss # Banner de frete grátis
        ├── _checkout.scss  # Seção de checkout / garantia
        ├── _faq.scss       # Seção de perguntas frequentes
        └── _footer.scss    # Rodapé
```

## Seções da Página

| Seção | Descrição |
|---|---|
| **Hero** | Headline principal, benefícios e CTA |
| **Pricing** | Planos de 2, 3 e 6 frascos com barra de confiança |
| **Formula** | Apresentação da fórmula e diferenciais |
| **Ingredients** | Cards com os 6 ingredientes principais |
| **Offer** | Seção de oferta com benefícios detalhados |
| **Testimonials** | Depoimentos de clientes reais |
| **Shipping Banner** | Destaque para frete grátis no plano de 6 frascos |
| **Checkout** | Grid de planos + caixa de garantia de 60 dias |
| **FAQ** | Accordion com perguntas frequentes + imagem da tabela nutricional |
| **Footer** | Links legais, disclaimer e copyright |

## Tecnologias

- **HTML5** semântico com BEM para nomenclatura de classes
- **SCSS/Sass** com arquitetura de partials (`@use`)
- **JavaScript** vanilla (ES6+)

## Pré-requisitos

- [Node.js](https://nodejs.org/) (para usar o Sass via npx)
- ou [Sass](https://sass-lang.com/install) instalado globalmente

## Como Usar

### Compilar o SCSS

```bash
npx sass src/scss/style.scss css/style.css
```

### Compilar com watch (recompila automaticamente ao salvar)

```bash
npx sass --watch src/scss/style.scss css/style.css
```

### Abrir a página

Abra o arquivo `index.html` diretamente no navegador ou use uma extensão como [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) no VS Code.

## Convenções de Código

- **BEM** — todas as classes seguem o padrão `bloco__elemento--modificador`
- **SCSS partials** — cada seção tem seu próprio arquivo `_nome.scss`
- **Variáveis centralizadas** — todas as cores estão em `_variables.scss` como fonte única da verdade
- **Mixins reutilizáveis** — padrões repetidos (barras de badge, separadores) estão em `_mixins.scss`
- **Componentes compartilhados** — `.btn`, `.fire-badge` e similares ficam em `_components.scss`

## Responsividade

Breakpoints utilizados:

| Breakpoint | Alvo |
|---|---|
| `max-width: 991px` | Tablets |
| `max-width: 768px` | Mobile |

Link do github pages:  
https://marciodouglasx.github.io/desafio-xmx/

Vídeo do desafio 


https://github.com/user-attachments/assets/cbe873a5-fc8b-4775-9ea6-0dc5cd1ec644



