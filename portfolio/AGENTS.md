# AGENTS.md — Regras Gerais de Desenvolvimento

Este documento define as diretrizes, restrições e padrões técnicos para o desenvolvimento do portfólio pessoal de **Lucas Fernandes da Silva**.

---

## 1. Princípios Fundamentais

1. **Stack Tecnológica Estrita**:
   - **HTML5 Semântico**: Uso de `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`.
   - **CSS3 Puro**: Vanilla CSS com variáveis CSS (design tokens), Flexbox, CSS Grid, microinterações e transições fluidas. Proibido TailwindCSS, Bootstrap ou frameworks CSS externos.
   - **JavaScript Puro (ES6+)**: Vanilla JS modular, sem jQuery ou frameworks como React/Vue/Angular.
2. **Fidelidade à Identidade Visual**:
   - Paleta de cores oficial (Preto azulado `#080B12`, Cinza escuro `#111827`, Azul-claro `#8ECFFF`, Azul vibrante `#398BFF`, Branco `#F5F7FA`, Cinza claro `#A7B0C0`).
   - Tipografia oficial: **Space Grotesk** para títulos e **Inter** para textos.
   - Estética futurista, elegante, limpa e com toques de iluminação/glow e glassmorphism refinado.
3. **Veracidade e Integridade dos Dados**:
   - **NÃO inventar** experiências profissionais, cargos fictícios, cursos não informados, certificados ou dados de contato fictícios.
   - Representar com precisão o perfil de Lucas: estudante interessado em tecnologia, com foco em aprendizado contínuo e desenvolvimento de projetos práticos.
4. **Links e Integrações Obrigatórias**:
   - **TCC CelsLife**: Deve apontar obrigatoriamente para `https://celslife.com.br/` abrindo em nova aba (`target="_blank"` com `rel="noopener noreferrer"`).
   - **GitHub**: Deve possuir uma variável única e centralizada no JavaScript (`PORTFOLIO_CONFIG.githubUrl`), claramente sinalizada para fácil customização pelo proprietário, sem inventar URL fictícia como fato consumado.
   - **Formulário de Contato**: Validação estrita via JS. Não simular envio falso (não fingir que enviou com backend se não houver backend real). Preparar a estrutura para integração real (ex: Formspree, EmailJS ou API própria) e exibir mensagem explicativa orientando a integração.

---

## 2. Acessibilidade e Performance

- Contraste visual aderente às diretrizes WCAG AA/AAA para texto claro sobre fundos escuros.
- Foco visível (`:focus-visible`) para navegação por teclado em todos os botões e links.
- Atributos ARIA adequados (`aria-label`, `aria-expanded`, `aria-hidden`, etc.).
- Suporte a `@media (prefers-reduced-motion: reduce)` para desabilitar ou suavizar animações para usuários sensíveis a movimento.
- Código leve, sem dependências pesadas externas, com carregamento otimizado de fontes.

---

## 3. Estrutura de Arquivos

```
portfolio/
├── AGENTS.md          # Este arquivo de regras
├── referencias.md     # Inspirações e diretrizes visuais
├── identidade.md      # Identidade visual, tipografia e biografia oficial
├── funcionalidades.md # Especificação funcional e fases
├── index.html         # Estrutura HTML da aplicação
├── style.css          # Estilos, tokens, layouts e responsividade
└── script.js          # Lógica, interações, validação e configuração
```

---

## 4. Metodologia de Desenvolvimento por Etapas

O desenvolvimento deve ser executado rigorosamente fase por fase, aguardando aprovação do usuário a cada entrega:

1. **Etapa 1**: Criação dos documentos base, configuração da estrutura inicial e desenvolvimento exclusivo da seção Hero e Header/Menu.
2. **Etapa 2**: Desenvolvimento da seção "Sobre Mim" com os 3 pilares visuais.
3. **Etapa 3**: Desenvolvimento da seção "Meus Projetos" com o card de destaque do TCC CelsLife e botão GitHub configurável.
4. **Etapa 4**: Desenvolvimento da seção "Contato" com formulário validado em JS e orientações de integração.
5. **Etapa 5**: Rodapé, ano dinâmico, polimento de animações, revisão de acessibilidade, testes de responsividade e correção de links.
