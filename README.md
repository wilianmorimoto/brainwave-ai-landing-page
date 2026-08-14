# Brainwave - AI Landing Page

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

O **Brainwave** é uma landing page de alta performance desenvolvida para a apresentação de um produto de Inteligência Artificial (SaaS). O objetivo principal do projeto foi criar uma interface visualmente impactante, com estética futurista e experiência de usuário fluida, demonstrando a aplicação de técnicas modernas de desenvolvimento frontend.

## 🚀 Tecnologias Utilizadas

O projeto foi construído com foco em performance e manutenibilidade, utilizando as seguintes ferramentas:

- **Core:** [React 18](https://react.dev/) com [Vite](https://vitejs.dev/) para um build extremamente rápido e HMR eficiente.
- **Estilização:** [Tailwind CSS](https://tailwindcss.com/) para a criação de layouts responsivos e design system consistente.
- **Interações Visuais:** [react-just-parallax](https://github.com/pavel-kuznetsov/react-just-parallax) para a implementação de efeitos de profundidade e imersão.
- **Navegação:** [react-router-dom](https://reactrouter.com/) para gestão de rotas e navegação interna.
- **Utilitários:** `scroll-lock` para controle de overflow em elementos de interface.

## 🛠️ Instalação e Execução

Para rodar o projeto localmente, siga os passos abaixo:

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/brainwave.git
   cd brainwave
   ```

2. **Instale as dependências:**
   ```bash
   npm install
   # ou
   pnpm install
   ```

3. **Inicie o servidor de desenvolvimento:**
   ```bash
   npm run dev
   ```

O projeto estará disponível em `http://localhost:5173`.

## 🧠 Engenharia de Frontend

### Arquitetura Orientada a Dados (Data-Driven)
Para garantir a escalabilidade e a facilidade de manutenção, implementei uma separação rigorosa entre a lógica de apresentação e a camada de dados. Todo o conteúdo textual, pricing, roadmap e links sociais estão centralizados em `src/constants/index.js`. Essa estratégia permite a atualização de todo o ecossistema da página sem a necessidade de alterar a estrutura dos componentes JSX, simulando o comportamento de um CMS.

### Estratégia de Design System & UI
- **Tailwind Customizado:** Implementação de um tema proprietário via `tailwind.config.js`, definindo paletas de cores e extensões específicas para manter a consistência visual e a estética futurista do produto.
- **SVGs como Componentes React:** Em vez de assets estáticos, elementos complexos como `ButtonGradient` e `SectionSvg` foram implementados como componentes. Isso permite maior controle sobre a renderização, otimização de performance e flexibilidade de estilização.
- **Experiência Imersiva com Parallax:** Utilização estratégica de `react-just-parallax` para criar camadas de profundidade, transformando a navegação linear em uma experiência visual dinâmica e imersiva.

### Composição de Componentes e Performance
- **Padronização Atômica:** O projeto foi estruturado em componentes independentes e reutilizáveis, facilitando a manutenção e a leitura do código.
- **Otimização de Assets:** Foco total em vetores (SVG) para garantir que a interface permaneça nítida em qualquer resolução (Retina/4K) enquanto mantém o tempo de carregamento reduzido.
- **Build Eficiente:** A escolha do Vite como build tool garante um ciclo de desenvolvimento rápido com HMR (Hot Module Replacement) e um bundle de produção extremamente otimizado.

## 📈 Performance e Boas Práticas

- **Otimização de Assets:** Uso de formatos SVG para ícones e elementos gráficos, reduzindo drasticamente o peso da página e mantendo a nitidez em qualquer resolução.
- **Build Otimizado:** Através do Vite, o projeto gera bundles minimizados e eficientes para produção.
- **Código Limpo:** Aplicação de padrões de nomenclatura semântica e organização de pastas intuitiva para facilitar o onboarding de novos desenvolvedores.

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
