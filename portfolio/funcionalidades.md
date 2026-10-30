# funcionalidades.md — Funcionalidades e Prioridades do Projeto

Este documento especifica os requisitos funcionais, a estrutura de cada seção e o plano de priorização e fases de entrega do portfólio.

---

## 1. Mapeamento de Funcionalidades

### A. Menu de Navegação (Header)
- Barra de navegação fixa no topo (`position: sticky` ou `fixed`).
- Logotipo / Marca com o nome "Lucas Fernandes" ou monograma minimalista.
- Links de âncora:
  - `Início` (`#inicio`)
  - `Sobre mim` (`#sobre`)
  - `Projetos` (`#projetos`)
  - `Contato` (`#contato`)
- Rolagem suave (`scroll-behavior: smooth`).
- Responsividade: Menu hambúrguer para dispositivos móveis com abertura fluida e acessível.
- Efeito visual de vidro com desfoque de fundo (`backdrop-filter`).

### B. Seção Hero (Página Inicial)
- **Título principal**: "Lucas Fernandes da Silva" em Space Grotesk com destaque tecnológico.
- **Badge tecnológica**: Elemento sutil indicando foco em tecnologia e desenvolvimento prático.
- **Frase principal**: *"Transformando curiosidade em conhecimento e conhecimento em projetos."*
- **Texto descritivo**: *"Sou um estudante interessado em tecnologia, sempre buscando aprender coisas novas, desenvolver minhas habilidades e transformar ideias em soluções práticas."*
- **Botões de Ação (CTAs)**:
  - Botão Primário: "Conheça meus projetos" (leva para `#projetos`).
  - Botão Secundário: "Entre em contato" (leva para `#contato`).
- **Composição Visual**: Grade geométrica de fundo com ponto de luz/glow dinâmico, animações suaves e visual arrojado.

### C. Seção Sobre Mim (Etapa 2)
- Título da seção: "Sobre mim".
- Texto biográfico humanizado e focado em aprendizado e evolução técnica.
- 3 cards de destaques visuais:
  1. **Aprendizado contínuo**
  2. **Interesse por tecnologia**
  3. **Desenvolvimento de projetos**
- Ícones em SVG e bordas com iluminação sutil.

### D. Seção Meus Projetos (Etapa 3)
- Título da seção: "Meus projetos".
- Card principal do TCC:
  - **Nome**: CelsLife
  - **Descrição**: *"Projeto de Trabalho de Conclusão de Curso, desenvolvido para colocar conhecimentos em prática e apresentar uma solução por meio de uma plataforma própria."*
  - **Ação**: Botão "Acessar meu TCC" apontando para `https://celslife.com.br/` com `target="_blank"`.
- Card de destaque do Repositório AG4:
  - **Nome**: AG4
  - **Descrição**: *"Acesse este repositório para conferir o projeto e seus arquivos."*
  - **Ação**: Botão "Ver projeto no GitHub" apontando para `https://github.com/vercellogo-alt/AG4` com `target="_blank"`.
- Botões "Meu GitHub" integrados no menu de navegação e na seção de contato.
- Link centralizado e configurável em uma única constante no arquivo `script.js` (`PORTFOLIO_CONFIG.githubUrl`).
- Arquitetura de código pronta para adicionar novos cards de projetos futuros sem refatoração.

### E. Seção Entre em Contato (Etapa 4)
- Título: "Entre em contato".
- Mensagem: *"Tem alguma ideia, oportunidade ou quer trocar conhecimentos? Entre em contato comigo!"*
- Formulário com campos:
  - Nome completo (validação: obrigatório, mínimo 3 caracteres).
  - E-mail (validação: obrigatório, formato de e-mail válido com regex).
  - Mensagem (validação: obrigatória, mínimo 10 caracteres).
  - Botão "Enviar mensagem".
- Validação no lado do cliente em JavaScript com feedback visual em tempo real e mensagens acessíveis.
- Aviso transparente explicando a ausência de backend ativo e orientando como conectar a serviços como Formspree, EmailJS ou API dedicada.
- Link de acesso ao GitHub.

### F. Rodapé (Etapa 5)
- Nome do autor: Lucas Fernandes da Silva.
- Ano atual gerado dinamicamente via JavaScript (`new Date().getFullYear()`).
- Links rápidos de navegação repetindo as seções principais.

---

## 2. Cronograma de Execução e Prioridades

| Etapa | Escopo | Status |
| :--- | :--- | :--- |
| **Etapa 1** | Arquivos de documentação (`AGENTS.md`, `referencias.md`, `identidade.md`, `funcionalidades.md`), estrutura base (`index.html`, `style.css`, `script.js`), Header de navegação e Seção Hero completa. | **Em Execução** |
| **Etapa 2** | Seção "Sobre Mim" com os 3 cards de destaque e layout responsivo. | Aguardando Etapa 1 |
| **Etapa 3** | Seção "Meus Projetos" com Card do CelsLife, botão GitHub configurável e grid escalável. | Aguardando Etapa 2 |
| **Etapa 4** | Seção de Contato com validação completa em JavaScript e guia de integração. | Aguardando Etapa 3 |
| **Etapa 5** | Rodapé dinâmico, animações adicionais, auditoria de acessibilidade, testes responsivos e encerramento. | Aguardando Etapa 4 |
