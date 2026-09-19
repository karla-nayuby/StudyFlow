# 📚 StudyFlow - Organização Inteligente de Estudos

> **StudyFlow** é uma aplicação web progressiva e acessível projetada para ajudar estudantes a organizarem suas rotinas acadêmicas, gerenciarem trabalhos com prazos e prioridades, e acompanharem o progresso de estudos com baixa carga cognitiva.

---

## 🎯 Apresentação do Case de Portfólio (UI / UX / Front-end)

### 1. Visão Geral do Produto
O StudyFlow resolve o problema da desorganização e do excesso de prazos acumulados enfrentado por estudantes. Ele oferece uma interface limpa, com navegação clara, dashboard visual e resposta tátil/interativa imediata para todas as ações do usuário.

---

### 2. Decisões de Design (UI & UX)

* **Baixa Carga Cognitiva:** Aplicação direta do conceito de *Progressive Disclosure*, mostrando informações consolidadas no Dashboard e detalhes sob demanda.
* **Hierarquia Visual Claramente Definida:** Uso de cartões com bordas coloridas indicando a matéria associada, *badges* com código de cores para prioridades (Alta, Média, Baixa) e tipografia escalada (Google Fonts - *Inter*).
* **Heurísticas de Nielsen Aplicadas:**
  1. *Visibilidade do status do sistema:* Barras de progresso dinâmicas e Notificações (Toasts) a cada ação efetuada.
  2. *Correspondência entre o sistema e o mundo real:* Uso de ícones universais da biblioteca Lucide.
  3. *Controle e liberdade do usuário:* Modais de confirmação e ações simples para excluir ou alterar dados.
  4. *Prevenção de erros:* Validação de formulários nativa e suporte a estados vazios explicativos.

---

### 3. Acessibilidade (WCAG 2.1)

* **Navegação via Teclado & Focus Visible:** Implementado um link visível no topo (*Skip Link*) para pular direto ao conteúdo principal. Todos os elementos interativos contam com anéis de foco (`:focus-visible`).
* **Suporte a Leitores de Tela:** Estruturação semântica em HTML5 (`<nav>`, `<main>`, `<header>`, `role="dialog"`, atributos `aria-label` e `aria-live`).
* **Áreas de Toque Adequadas:** Todos os botões e áreas interativas possuem dimensão mínima de `48px x 48px`, ideal para uso mobile e acessibilidade tátil.
* **Contraste de Cores:** Atende aos requisitos mínimos de contraste de cores do padrão WCAG AA tanto no modo Claro quanto no Dark Mode.

---

### 4. Recurso Tátil & Gestos Mobile

* **Swipe Right:** Deslize o dedo sobre uma tarefa para alternar seu status entre concluída e pendente.
* **Long Press:** Pressione e segure um item de tarefa para abrir o atalho rápido de exclusão.
* **Feedback Háptico:** Integração com a API `navigator.vibrate` para dar resposta física nos dispositivos touch a cada ação concluída.

---

### 5. Segurança & Biometria

* **Anotações Privadas Protegidas:** Implementação de simulação/integração com a API `WebAuthn` (Biometria nativa / Touch ID / Face ID) para proteger blocos de anotações confidenciais do estudante.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 Semântico**
* **CSS3 Moderno** (Flexbox, CSS Grid, Variáveis CSS, Dark Theme)
* **JavaScript Puro (ES6+)** (Gerenciamento de Estado, Manipulação de DOM, LocalStorage)
* **Lucide Icons** (Ícones SVG Leves)
* **Web APIs Nativas:** `Vibration API`, `WebAuthn API`, `LocalStorage API`

---

## 🚀 Como Executar o Projeto

1. Baixe o arquivo `index.html`.
2. Abra o arquivo diretamente em qualquer navegador moderno (Chrome, Firefox, Safari, Edge).
3. Para testar a responsividade e gestos touch, abra as **Ferramentas do Desenvolvedor** (`F12`) e ative a visualização de dispositivos móveis.
