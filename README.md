<div align="center">

# Blocos Semânticos em Inglês

**Material didático interativo para brasileiros aprenderem inglês em blocos de uso real**

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-blocos--semanticos--em--ingles-0D9488?style=for-the-badge)](https://blocos-semanticos-em-ingles.netlify.app/)
[![PWA](https://img.shields.io/badge/PWA-Installable-D4A843?style=for-the-badge&logo=pwa)](https://blocos-semanticos-em-ingles.netlify.app/)
[![License](https://img.shields.io/badge/License-Proprietary-64748B?style=for-the-badge)](#-licença)

*Um produto [VS Consulting™](#-sobre-a-vs-consulting)*

</div>

---

## 🎯 Sobre o projeto

**Blocos Semânticos em Inglês** é uma plataforma web interativa que ensina inglês de forma **contextual e pragmática** — não através de regras gramaticais isoladas, mas via **230 "blocos de construção" semânticos** que nativos usam em situações reais de comunicação.

A proposta parte de uma constatação simples: brasileiros que estudam inglês tradicionalmente acumulam vocabulário e gramática, mas travam na fluência porque não dominam **como os blocos de pensamento se encadeiam** — frases como *"I'm in the middle of something"*, *"That's a fair point, but..."* ou *"I've come a long way since..."* não são ensinadas em aulas convencionais, mas aparecem o tempo todo em conversas reais, reuniões e contextos profissionais.

### O que diferencia este material

- **Pensamento em blocos semânticos, não em palavras isoladas** — aprendizado por contexto e intenção comunicativa
- **Taxonomia cromática de 6 famílias** — cada bloco tem uma "função social" (Social, Emotional, Cognitive, Action, Temporal, Discursive)
- **Tradução pragmática para brasileiros** — não literal, mas com equivalência de registro e intenção
- **Pronúncia acessível** — IPA + transcrição fonética amigável para falantes de português
- **Design editorial refinado** — tema dark/light, tipografia serif/sans contrastante, foco em leitura

---

## ✨ Funcionalidades

### 📚 Conteúdo didático
- **230 blocos semânticos** organizados em **29 categorias** temáticas
- **3 níveis de dificuldade** — Basic, Intermediate, Advanced
- **3 exemplos contextualizados** por bloco, com traduções pragmáticas
- **Slots de variação** — palavras/expressões intercambiáveis para construir combinações
- **Insight pedagógico** — dica de uso ao final de cada bloco
- **Blocos relacionados** — navegação em rede via similaridade semântica

### 🗣️ Pronúncia completa
- **Transcrição IPA** (Alfabeto Fonético Internacional)
- **Divisão silábica** marcada com pontos
- **Marcação de ênfase** em MAIÚSCULAS
- **Transcrição amigável** adaptada para leitores brasileiros
- **Dica de pronúncia** em português para cada bloco
- **Áudio TTS** (Text-to-Speech) para o padrão principal + 3 exemplos = **4 botões de áudio por bloco** (**920 pontos de reprodução** no total)

### 🎨 Experiência de uso
- **Design responsivo mobile-first** — funciona de celular a widescreen
- **Tema dark/light** com persistência local
- **6 famílias cromáticas** — identificação visual da função semântica
- **Filtros combinados** — por família, categoria e nível (multi-select)
- **Busca em tempo real** — padrões, traduções e exemplos
- **Sistema de favoritos** com persistência local
- **Copy-to-clipboard** em cada exemplo
- **Export em PDF** dos blocos favoritados (layout editorial)
- **Micro-interações** refinadas em todas as ações

### 📱 PWA (Progressive Web App)
- **Instalável** na tela inicial do celular
- **Funciona offline** após primeira visita
- **Abre em tela cheia** — experiência de app nativo
- **Ícone personalizado** em formato Android/iOS/desktop
- **Sem necessidade de loja de apps**

---

## 🎨 Sistema de Design

### Tipografia

| Fonte | Uso |
|---|---|
| **Playfair Display** | Títulos, padrões em inglês, branding (serif editorial) |
| **IBM Plex Sans** | Corpo de texto, interface (sans-serif humanista) |
| **JetBrains Mono** | IPA, transcrições fonéticas, versioning (monoespaçada técnica) |

### Paleta de Famílias Semânticas

| Família | Cor | Função comunicativa |
|---|---|---|
| 🟠 **Social** | `#F97316` Coral | Interação humana, gentilezas, fechamentos |
| 🌹 **Emotional** | `#F472B6` Rose | Estados internos, sentimentos, desejos |
| 💜 **Cognitive** | `#A78BFA` Violet | Opinião, argumentação, pensamento crítico |
| 🟡 **Action** | `#FBBF24` Amber | Capacidade, obrigação, compromisso |
| 🟢 **Temporal** | `#34D399` Emerald | Tempo, narrativa, sequência |
| 🔵 **Discursive** | `#38BDF8` Sky | Estrutura do discurso, conectivos |

### Cores da marca

- **Navy** `#0A1628` — fundo principal (dark)
- **Gold** `#D4A843` — acentos editoriais, padrões em inglês
- **Teal** `#0D9488` — estado ativo, interatividade
- **Cream** `#F4F1EA` — fundo light theme

---

## 🛠️ Arquitetura técnica

### Stack

- **HTML5** — estrutura semântica, sem frameworks
- **CSS3 puro** — CSS Variables, Grid, Flexbox, `@media` queries, `@container`, `color-mix()`
- **JavaScript vanilla (ES2020+)** — sem build step, sem dependências externas
- **Web APIs nativas** — Speech Synthesis, Clipboard, localStorage, Service Worker, Web App Manifest

### Princípios de design de código

- **Zero dependências externas** (fontes via Google Fonts CDN apenas)
- **Progressive Enhancement** — funciona mesmo sem JS (conteúdo estático visível)
- **Graceful Degradation** — cada feature falha silenciosamente se não suportada
- **Single-file deployable** — `index.html` contém toda a aplicação

### Por que arquitetura assim?

O material é, antes de tudo, **um ativo didático distribuível**. A escolha por HTML/CSS/JS sem build permite:

1. **Portabilidade máxima** — funciona via `file://`, hosting estático, ou iframe embarcado
2. **Longevidade** — não depende de versões de Node, frameworks que deprecam, ou infraestrutura complexa
3. **Auditabilidade** — qualquer desenvolvedor inspeciona o código direto, sem source maps
4. **Performance** — um único HTML de ~350KB carrega em <1s mesmo em 3G
5. **Offline-first por design** — todo conteúdo (230 blocos + 230 pronúncias) embutido no JS

---

## 📦 Estrutura de arquivos

```
blocos-semanticos-ingles/
├── index.html              # Aplicação completa (HTML + CSS + JS + dados)
├── manifest.json           # Web App Manifest para PWA
├── icon-192.png            # Ícone PWA Android
├── icon-512.png            # Ícone PWA high-res
├── icon-maskable.png       # Ícone adaptativo Android
├── apple-touch-icon.png    # Ícone iOS Safari
├── favicon-32.png          # Favicon do navegador
└── README.md               # Este arquivo
```

---

## 🚀 Como executar localmente

### Opção 1 — Abrir direto no navegador

```bash
# Clone o repositório
git clone https://github.com/SEU-USUARIO/blocos-semanticos-ingles.git
cd blocos-semanticos-ingles

# Abra o index.html no navegador
open index.html  # macOS
xdg-open index.html  # Linux
start index.html  # Windows
```

> ⚠️ **Limitação do `file://`**: o PWA não instala via `file://` (requer HTTPS). Para testar PWA localmente, use a Opção 2.

### Opção 2 — Servidor local HTTPS

```bash
# Python 3 (servidor HTTP simples)
python3 -m http.server 8000

# Node.js (se preferir)
npx serve .

# Acesse em http://localhost:8000
```

Para PWA real, use ferramenta como `ngrok` para expor seu servidor local via HTTPS:
```bash
ngrok http 8000
```

### Opção 3 — Deploy em produção

Suba os arquivos diretamente em qualquer host estático:
- [Netlify](https://netlify.com) (gratuito, HTTPS automático)
- [GitHub Pages](https://pages.github.com)
- [Vercel](https://vercel.com)
- [Cloudflare Pages](https://pages.cloudflare.com)

---

## 📲 Como instalar como aplicativo

Acesse https://blocos-semanticos-em-ingles.netlify.app/ pelo navegador do celular:

### Android (Chrome)
1. Aguarde 2 segundos na página
2. Banner **"📲 Instalar aplicativo"** aparece na parte inferior
3. Toque em **"Instalar"**
4. Ícone **"Blocos EN"** aparece na tela inicial

*Alternativamente:* Chrome → menu **⋮** → **"Instalar aplicativo"**

### iOS (Safari)
1. Toque no botão **Compartilhar** (ícone ⬆️)
2. Role e selecione **"Adicionar à Tela de Início"**
3. Toque em **"Adicionar"** no canto superior direito

---

## 🧪 Testes e compatibilidade

### Navegadores suportados
- ✅ Chrome/Edge 90+ (desktop + mobile)
- ✅ Safari 15+ (desktop + iOS)
- ✅ Firefox 90+
- ✅ Samsung Internet 15+

### Features por contexto

| Feature | Hospedado HTTPS | Arquivo local | Iframe sandbox |
|---|---|---|---|
| 230 Blocos + IPA | ✅ | ✅ | ✅ |
| Pronúncia IPA local | ✅ | ✅ | ✅ |
| Áudio TTS | ✅ | ✅ | ⚠️ limitado |
| Copy to clipboard | ✅ | ✅ | ✅ |
| Theme toggle | ✅ | ✅ | ✅ |
| Favoritos | ✅ | ✅ | ✅ |
| Export PDF | ✅ | ✅ | ✅ |
| PWA instalável | ✅ | ❌ | ❌ |
| Offline support | ✅ | ✅ | ⚠️ limitado |

---

## 🎓 Guia de uso pedagógico

### Para auto-estudo
1. Comece pelo nível **Basic**, filtre por família que mais te interessa
2. Abra cada bloco, leia o padrão em inglês e português
3. Toque no botão **🔊** para ouvir a pronúncia
4. Toque no botão **🗣️** para ver o guia IPA completo
5. Expanda **"See examples"** para ver variações em contexto
6. Favorite os blocos que quer revisar depois
7. Ao completar uma família, exporte seus favoritos como PDF

### Para educadores
- Use os filtros combinados para criar **trilhas temáticas** em sala de aula
- O painel IPA funciona como **material de apoio** para ensino de pronúncia
- O export PDF permite entregar **materiais personalizados** para cada aluno
- Os "blocos relacionados" facilitam **aprendizado em rede** vs. linear

### Para consultores/profissionais
- Filtre pela família **Action + Discursive** para inglês corporativo
- Use os blocos de **"Business & Professional"** e **"Commitment & Promises"** para preparação de reuniões
- Os blocos **"Hedging & Softening"** são essenciais para diplomacia em inglês

---

## 🗺️ Roadmap

### ✅ Release atual — v3.2 (2025)
- 230 blocos semânticos completos
- Sistema de pronúncia IPA local
- Áudio TTS (pattern + 3 exemplos)
- Dark/light theme
- Blocos relacionados via similaridade
- Export PDF de favoritos
- PWA instalável
- Mobile-first responsivo

### 🛣️ Próximas versões (planejadas)
- **v3.3** — Modo "Study" com flashcards e repetição espaçada
- **v3.4** — Atalhos de teclado (`/` busca, `1/2/3` nível, `F` favoritos)
- **v3.5** — Pronunciation Challenge (gravação + comparação)
- **v4.0** — "Blocos Pro" — versão premium com +100 blocos de negócios
- **v4.1** — Analytics integrado (Plausible) e A/B de conteúdo
- **v4.2** — Domínio próprio (`blocos.vsconsulting.com.br`)

---

## 🤝 Contribuição

Este é um projeto **proprietário da VS Consulting™**, mas **feedback e sugestões são muito bem-vindos**.

### Como contribuir
- **Reportar erros** de pronúncia, tradução ou exemplo: abra uma [Issue](../../issues)
- **Sugerir novos blocos**: abra uma Discussion ou envie por [e-mail](#-contato)
- **Feedback de UX/pedagógico**: sempre apreciado

### Não aceito no momento
- Pull requests de código (o projeto é proprietário)
- Forks para redistribuição comercial

---

## 📝 Licença

**Proprietary © 2025 VS Consulting™.** Todos os direitos reservados.

Este material é disponibilizado **gratuitamente para uso pessoal e educacional**. É **permitido**:
- ✅ Usar o material para estudo pessoal
- ✅ Compartilhar o link com alunos, colegas, amigos
- ✅ Referenciar em aulas e palestras (com atribuição)

É **proibido**, sem autorização prévia por escrito:
- ❌ Redistribuir ou copiar o conteúdo dos blocos em outras plataformas
- ❌ Usar comercialmente (cobrar por acesso, incluir em produtos pagos)
- ❌ Modificar e republicar como próprio
- ❌ Remover a atribuição à VS Consulting™

Para licenciamento comercial ou uso institucional, entre em contato.

---

## 🏢 Sobre a VS Consulting

**VS Consulting™** é uma consultoria especializada em **estratégia, dados, tecnologia, automação, inteligência artificial e tomada de decisão de alto nível**, fundada por **Vagner Alves dos Santos**.

Este projeto é parte do portfólio de ativos didáticos da VS Consulting, demonstrando capacidade de entregar **soluções técnicas sofisticadas** em projetos que atravessam fronteiras entre educação, design, engenharia de software e consultoria estratégica.

### Áreas de atuação
- 📊 **Estratégia e análise de negócios** — frameworks de decisão, diagnósticos estratégicos, roadmaps executivos
- 🧠 **Inteligência artificial aplicada** — sistemas multiagentes, automação cognitiva, integração LLM
- 📈 **Dados e analytics** — dashboards executivos (Power BI/DAX), pipelines, modelagem estatística
- 🎯 **Produtos digitais** — plataformas educacionais, ferramentas de consulting, MVPs de alto impacto
- 🎓 **Materiais educacionais** — conteúdo técnico e executivo para formação continuada

---

## 📬 Contato

- **Site:** [blocos-semanticos-em-ingles.netlify.app](https://blocos-semanticos-em-ingles.netlify.app/)
- **LinkedIn:** [Vagner Alves dos Santos](https://linkedin.com/in/vagner-alves-dos-santos)
- **GitHub:** [@vagneralvesdossantos](https://github.com/)
- **E-mail:** *(adicione seu e-mail aqui)*

---

<div align="center">

**Construído com ❤️ e atenção obsessiva aos detalhes por [VS Consulting™](#-sobre-a-vs-consulting)**

*Se este material te ajudou, considere compartilhar com alguém que também queira destravar seu inglês.*

</div>
