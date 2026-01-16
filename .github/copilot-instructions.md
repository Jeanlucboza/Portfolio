# Instruções para Agentes de IA - Portfolio Front-end

## Visão Geral do Projeto

Este é um **portfolio pessoal de um desenvolvedor front-end** construído com HTML5, CSS3 e JavaScript puro. É uma aplicação web estática (sem backend) com foco em design responsivo, animações suaves e apresentação de projetos.

**Estrutura essencial:**
- `index.html`: Markup semântico em português com seções de header, projects e footer
- `style.css`: Estilos com gradientes, animações CSS e grid responsivo
- `assets/`: Imagens dos projetos (ex: `calculadora IMC.png`)

## Padrões e Convenções

### Design Visual
- **Gradiente Principal**: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)` - gradiente roxo em background
- **Cores**: `#667eea` (roxo primário), `#764ba2` (roxo secundário), branco para contraste
- **Animações CSS**: `fadeInDown`, `fadeInUp`, `fadeIn` com transições de 1s
- **Border Radius**: 15px para cards, 25px para botões de contato

### Grid Responsivo
- Desktop: `grid-template-columns: repeat(auto-fit, minmax(320px, 1fr))`
- Mobile: Header reduzido, grid collapsa para 1 coluna via media query `@media (max-width: 768px)`
- Cards de projeto fluem dinamicamente

### Componentes Principais
1. **Header**: Nome, subtítulo, descrição e links de contato com ícones emoji
2. **Projects Grid**: 3 cards (Landing Page, Conversor Moedas, Calculadora IMC) com tags de tecnologia
3. **Footer**: Copyright e mensagem decorativa

## Desenvolvimento e Manutenção

### Integração de Imagens
- Imagens em `assets/` são referenciadas via caminho relativo (`./assets/calculadora\ IMC.png`)
- Propriedades CSS para imagens: `background-size: contain`, `background-position: center`, `background-repeat: no-repeat`
- Note: Nomes com espaços requerem escape com barra invertida em URLs CSS

### Adicionar Novos Projetos
1. Duplicar `.project-card` em `index.html`
2. Atualizar títulos, descrições e tags de tecnologia
3. Adicionar imagem em `assets/` e referenciá-la
4. Links estão atualmente como `href="#"` - substituir por URLs reais quando disponível

### Idioma
- Conteúdo em **português brasileiro** (pt-BR)
- Meta charset e lang="pt-BR" já configurados
- Textos estão em português (ex: "Desenvolvedor Front-end", "Meus Projetos")

## Checklist para Contribuições

- [ ] Alterações visuais testadas em breakpoints 320px, 768px e desktop
- [ ] Animações mantêm duração de 1s para consistência
- [ ] Novas cores respeitam paleta roxa existente
- [ ] Imagens adicionadas em `assets/` com nomes descritivos em português
- [ ] Conteúdo em português brasileiro
