# 🤝 ONG Esperança - Plataforma Social Web

Uma plataforma web moderna, acessível e responsiva desenvolvida para a **ONG Esperança**, destinada à divulgação de projetos sociais, captação de doações e gestão de cadastros de voluntários.

---

## 📌 Sumário
- [Demonstração e Tecnologias](#-demonstração-e-tecnologias)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Arquitetura do Design System](#-arquitetura-do-design-system)
- [Acessibilidade (WCAG 2.1)](#-acessibilidade-wcag-21)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Autor](#-autor)

---

## 🚀 Demonstração e Tecnologias

A aplicação foi desenvolvida utilizando padrões modernos de desenvolvimento Front-end sem dependências complexas de frameworks, priorizando desempenho, semântica e acessibilidade.

### Tecnologias Utilizadas:
* **HTML5 Semântico**: Estruturação clara com suporte a atributos ARIA.
* **CSS3 Avançado**: Uso de variáveis nativas (*CSS Custom Properties*), CSS Grid de 12 colunas e Flexbox.
* **JavaScript ES6+**: Roteamento cliente (SPA), validações em tempo real e manipulação do DOM.
* **IMask.js**: Biblioteca leve para aplicação de máscaras dinâmicas em campos de input (CPF, CEP, Telefone).
* **LocalStorage**: Persistência de dados local diretamente no navegador.
* **GitHub Pages**: Hospedagem e deploy contínuo (CI/CD) via GitHub Actions.

---

## ⚡ Funcionalidades Principais

* 🔄 **Arquitetura SPA (Single Page Application)**: Navegação fluida sem *refresh* de página entre as abas Início, Projetos e Cadastro.
* 🌗 **Modo Escuro / Alto Contraste (Dark Mode)**: Suporte a troca de tema claro/escuro com salvamento da preferência do usuário no `localStorage`.
* 📋 **Formulário com Validação em Tempo Real**:
  * Aplicação de RegEx para validação de e-mail, CPF, telefone e CEP.
  * Injeção dinâmica de mensagens de erro no DOM.
  * Máscaras de formatação automática para inputs sensíveis.
* 💾 **Persistência de Cadastros**: Salvamento dos dados preenchidos no `localStorage` em formato JSON.
* 📱 **Layout Totalmente Responsivo**: Grade adaptativa testada em 5 *breakpoints* distintos (Mobile Extra Small, Mobile, Tablet, Desktop e Ultra-Wide).

---

## 🎨 Arquitetura do Design System

O projeto conta com um Design System estruturado com variáveis CSS nativas (`:root`), abrangendo:

1. **Paleta de 8 Cores Distintas**:
   * Primárias: Azul Escuro (`#1E3A8A`) / Azul Vibrante (`#1D4ED8`)
   * Secundárias: Verde Esmeralda (`#0D9488`) / Verde Escuro (`#0F766E`)
   * Neutras: Escuro (`#1F2937`), Médio (`#4B5563`), Claro (`#F3F4F6`), Branco (`#FFFFFF`)
2. **Escala Tipográfica Modular**: 5 níveis hierárquicos baseados em `rem` (`h1`, `h2`, `h3`, `body`, `small`).
3. **Escala de Espaçamento Modular**: Sistema baseado em múltiplos de 8px (`8px`, `16px`, `24px`, `32px`, `48px`).

---

## ♿ Acessibilidade (WCAG 2.1)

O desenvolvimento priorizou os critérios de acessibilidade diretrizes WCAG AAA:
* **Contraste Mínimo**: Taxa superior a 7:1 para todos os textos e elementos de interface.
* **Navegação por Teclado**: Estados de foco visíveis (`:focus-visible`) com `outline` em destaque.
* **Atributos ARIA**: Rótulos e avisos dinâmicos (`role="alert"`, `aria-label`, `role="status"`) para leitores de tela.

---

## 📂 Estrutura do Projeto

```text
/
├── index.html        # Página principal e container da SPA
├── projetos.html     # Aba de listagem de projetos sociais
├── cadastro.html     # Formulário de cadastro de voluntários
└── assets/
    └── images/       # Imagens e logotipos da organização
