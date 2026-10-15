# 🎬 MovieCity — Plataforma de Cinema de Próxima Geração

Uma experiência cinematográfica imersiva e de **altíssimo desempenho**, desenvolvida com **React 19**, **Vite 7** e **CSS3 moderno de alta fidelidade**. Projetada com estética *cyber-dark/A24*, iluminação dinâmica com reflexos de aura ambiente, sintetizador de som nativo via **Web Audio API**, persistência de dados em **LocalStorage** e zero dependências pesadas externas.

---

## ⚡ Tecnologias & Arquitetura de Alto Desempenho

- **React 19**: Renderização ultra rápida, estado reativo com `useMemo` e `useCallback` para busca e filtros sem re-renderizações desnecessárias.
- **Vite 7**: Ambiente de desenvolvimento instantâneo e bundling com sub-100ms de carregamento.
- **Web Audio API**: Efeitos sonoros táteis e procedurais (clique, favoritar, nota de avaliação e abertura de modal) sintetizados dinamicamente pelo navegador, sem necessidade de carregar arquivos de áudio pesados, com controle liga/desliga de mudo.
- **LocalStorage Persistence Engine**: Sincronização automática e persistência da *Minha Lista (Watchlist)*, notas de avaliações dos filmes e perfil de usuário.
- **Sistema Vetorial SVG Inline Nativo**: Coleção completa de ícones em SVG puro, sem bibliotecas externas pesadas, garantindo fidelidade visual e tempo de resposta zero.
- **CSS3 GPU-Accelerated & Glassmorphism**: Utilização de `backdrop-filter`, `clamp()` para tipografia fluida, `will-change` e transformações 3D aceleradas por hardware para 60/120 FPS estáveis.

---

## ✨ Funcionalidades Principais

1. **Billboard Cinematográfico (Hero Carousel)**:
   - Carrossel com os principais destaques, temporizador automático (pausa ao passar o mouse) e troca instantânea de títulos.
   - Pôster em alta resolução com iluminação de aura ambiente calculada na cor do filme.
   - Botões de ação rápida: Assistir Trailer, Minha Lista e Detalhes do Filme.
   - Miniaturas inferiores interativas para pré-visualização em 1 clique.

2. **Player de Trailer Cinematográfico (Modo Cinema)**:
   - Modal em tela ampla com efeito de luz ambiente traseira (*Backlight Ambient Glow*).
   - Especificações de vídeo (4K Ultra HD, Dolby Vision, Som Espacial).
   - Atalho de teclado `ESC` para fechamento instantâneo.

3. **Catálogo Inteligente com Busca e Filtros em Tempo Real**:
   - Barra de busca instantânea com atalho global `/` (pressione `/` para focar imediatamente na busca).
   - Filtro por categorias com contadores dinâmicos de títulos disponíveis.
   - Filtro de pontuação mínima (ex: `★ 8.0+`, `★ 9.0+`).
   - Ordenação inteligente: *Mais Populares*, *Melhor Avaliados*, *Lançamentos Recentes* e *A-Z*.
   - Alternador de visualização: Grade de Pôsteres vs. Lista Detalhada Compacta.

4. **Gaveta Deslizante "Minha Lista" (Watchlist Drawer)**:
   - Gaveta lateral animada exibindo todos os filmes favoritados.
   - Acesso direto ao trailer ou detalhes de cada título.
   - Remoção individual ou limpeza completa com persistência no navegador.

5. **Modal de Detalhes com 4 Abas**:
   - **Visão Geral**: Sinopse completa, ficha técnica de produção (direção, áudio, resolução, faixa etária).
   - **Widget Interativo de Avaliação**: O usuário pode votar de 1 a 5 estrelas interativamente e salvar sua nota.
   - **Elenco & Personagens**: Cartões com avatares dos atores e papéis interpretados.
   - **Comentários da Comunidade**: Formulário para publicação de novas análises e lista de resenhas.
   - **Títulos Semelhantes**: Sugestões automáticas baseadas no mesmo gênero.

6. **Sistema de Autenticação & Perfil**:
   - Abas de "Entrar" e "Criar Conta".
   - Botão **"Testar com Usuário Demo"** para preenchimento em 1 clique.
   - Perfil logado exibindo avatar, nome de usuário, selo VIP PRO e menu de configurações/logout.

7. **Notificações Toast Flutuantes**:
   - Notificações instantâneas com barra de contagem regressiva para ações como salvar na lista, avaliar um filme ou fazer login.

---

## ⌨️ Atalhos de Teclado

| Tecla | Ação |
| :---: | :--- |
| `/` | Foca instantaneamente na barra de busca de filmes |
| `Esc` | Fecha qualquer modal, gaveta ou player ativo |

---

## 🚀 Como Executar

1. Abra a pasta do projeto no VS Code ou terminal:
   ```bash
   npm install
   ```
2. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```
3. Acesse o endereço exibido no terminal (geralmente `http://localhost:5173`).

---

## 📁 Estrutura do Projeto

```text
MovieCity/
├── public/
├── src/
│   ├── assets/                 # Pôsteres e capas dos filmes
│   ├── components/
│   │   ├── AuthModal.jsx       # Modal de login/cadastro com preenchimento demo
│   │   ├── Footer.jsx          # Rodapé com newsletter e stack tecnológica
│   │   ├── Header.jsx          # Navbar com busca, áudio, lista e perfil
│   │   ├── HeroBanner.jsx      # Billboard em destaque com carrossel dinâmico
│   │   ├── Home.jsx            # Orquestrador de estado e layout
│   │   ├── Icons.jsx           # Ícones SVG nativos e ultraleves
│   │   ├── MovieCard.jsx       # Cartão do filme com hover 3D e ações
│   │   ├── MovieDetailsModal.jsx # Modal com abas, elenco e avaliação
│   │   ├── MovieGrid.jsx       # Catálogo, busca, filtros e ordenação
│   │   ├── Toast.jsx           # Sistema de notificações flutuantes
│   │   ├── TrailerPlayerModal.jsx # Player de cinema com backlight
│   │   └── WatchlistDrawer.jsx # Gaveta lateral da lista de favoritos
│   ├── data/
│   │   └── moviesData.js       # Catálogo expandido com metadados e resenhas
│   ├── utils/
│   │   ├── audio.js            # Efeitos sonoros via Web Audio API
│   │   └── storage.js          # Sincronização persistente com LocalStorage
│   ├── App.jsx
│   ├── index.css               # Arquitetura CSS completa e responsiva
│   └── main.jsx
├── index.html                  # Fontes Google, SEO e Favicon SVG
├── package.json
└── vite.config.js
```

© 2026 MovieCity · Todos os direitos reservados.
