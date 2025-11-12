# 📚 Documentação UX/UI - AutoPrime

---

## 📋 Índice
1. [Princípios de Robin Williams](#1-princípios-de-robin-williams)
2. [Leis do Design](#2-leis-do-design)
3. [Heurísticas de Nielsen](#3-heurísticas-de-nielsen)
4. [Vieses Cognitivos](#4-vieses-cognitivos)
5. [IHC - Interação Humano-Computador](#5-ihc)

---

## 1. Princípios de Robin Williams

### 🔹 PROXIMIDADE
Elementos relacionados devem estar próximos.

**Aplicações:**
- **Header**: Logo, contatos e busca agrupados
- **Contact Info**: Links de contato agrupados com `gap: 20px`
- **Vehicle Info**: Título, detalhes e preço juntos no card

### 🔹 ALINHAMENTO
Nada deve ser colocado arbitrariamente.

**Aplicações:**
- **Navigation**: Menu centralizado com `justify-content: center`
- **Hero Content**: Conteúdo centralizado vertical e horizontalmente
- **Section Titles**: Títulos centralizados

### 🔹 REPETIÇÃO
Repetir elementos visuais em todo o material.

**Aplicações:**
- **Links**: Padrão consistente para todos os links do header
- **Cards**: Todos os cards de veículos seguem o mesmo padrão
- **Buttons**: CTAs com o mesmo estilo de gradiente

### 🔹 CONTRASTE
Fazer elementos diferentes realmente diferentes.

**Aplicações:**
- **Logo**: Branco sobre gradiente roxo
- **Search Button**: Laranja destacado `#f39c12`
- **Vehicle Price**: Preço em roxo grande `font-size: 24px`

---

## 2. Leis do Design

### 🔹 LEI DE FITTS
Alvos maiores e mais próximos são mais fáceis de acertar.

**Aplicações:**
- **Botões**: `padding: 6px 12px` para área clicável adequada
- **Navigation**: `padding: 18px 25px` em links de menu
- **Mobile**: Botões ainda maiores no mobile

### 🔹 LEI DE HICK
Mais opções = mais tempo de decisão.

**Aplicações:**
- **Menu (HTML)**: Apenas 6 itens no menu principal
- **Search**: Um único campo de busca simplificado

### 🔹 LEI DE MILLER (7±2)
Limite de 7±2 itens na memória de trabalho.

**Aplicações:**
- **Navigation**: 6 itens (Home, Estoque, Avaliação, Financiamento, Empresa, Contato)
- **Hero Stats**: 3 estatísticas apenas
- **Features**: 3 features principais

### 🔹 LEI DA GESTALT

**Similaridade**: Cards similares são percebidos como grupo
**Região Comum**: Cards com fundo branco formam unidades visuais
**Simetria**: Grid simétrico 4 colunas

---

## 3. Heurísticas de Nielsen


### ✅ 1. Correspondência com Mundo Real
- **Labels**: "Home", "Estoque", "Contato" - linguagem familiar
- **Icons**: Telefone, WhatsApp, mapa - ícones reconhecíveis

### ✅ 2. Consistência e Padrões
- **Colors**: Paleta roxo/laranja consistente em todo site
- **Transitions**: Todas em `0.3s ease`
- **Border Radius**: Todos os cards com `12px`

### ✅ 4. Reconhecimento ao Invés de Memorização
- **Icons**: Ícones grandes de 48px para fácil reconhecimento
- **Badge "OFERTA"**: Visualmente destacado

### ✅ 5. Design Estético e Minimalista
- **Cards**: Apenas informações essenciais
- **Layout limpo**: Muito espaço em branco

---

## 4. Vieses Cognitivos

### 🧠 PROVA SOCIAL
**Onde:** Hero Stats
```html
500+ Veículos Vendidos
100% Procedência
10+ Anos de Experiência
```
**Por quê:** Demonstra credibilidade e confiança

### 🧠 ESCASSEZ
**Onde:** Badge "OFERTA"
```css
.vehicle-badge {
  animation: pulse 2s infinite;
}
```
**Por quê:** Cria senso de urgência

### 🧠 ANCORAGEM
**Onde:** Preço antigo
```html
<p class="old-price">de R$ 55.900</p>
<div class="vehicle-price">R$ 53.900</div>
```
**Por quê:** Faz o preço atual parecer melhor negócio

### 🧠 AUTORIDADE
**Onde:** Feature Icons
```html
<i class="fas fa-shield-alt"></i>
100% Procedência
```
**Por quê:** Ícone de escudo transmite segurança e confiança

---

## 5. IHC

### 💡 FEEDBACK VISUAL
**Aplicações:**
- **Hover cards**: `transform: translateY(-10px)` ao passar mouse
- **Button active**: `transform: scale(0.98)` ao clicar

### 💡 AFFORDANCE
Elementos que indicam como usá-los:
- **Cursor pointer**: Indica clicabilidade
- **Button gradients**: Sombras indicam que é clicável
- **Hover effects**: Mudanças visuais mostram interatividade

### 💡 ACESSIBILIDADE
- **VLibras**: Plugin para pessoas surdas (HTML)
- **UserWay**: Ferramentas de acessibilidade (HTML)
- **ARIA labels**: Em todos elementos interativos
- **Semantic HTML**: `<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`
- **Loading lazy**: `<img loading="lazy">` para performance

### 💡 NAVEGAÇÃO INTUITIVA
- **Sticky nav**: `position: sticky` - sempre disponível
- **Smooth scroll**: `scroll-behavior: smooth`
- **Active state**: Mostra onde usuário está


---

## 🎯 Principais Destaques

### Design Visual
- ✅ Paleta de cores consistente (roxo + laranja)
- ✅ Hierarquia visual clara
- ✅ Espaçamento harmônico
- ✅ Contraste adequado

### Usabilidade
- ✅ Navegação intuitiva
- ✅ Layout responsivo (3 breakpoints)
- ✅ Performance otimizada

### Psicologia
- ✅ Prova social com números
- ✅ Escassez com badges
- ✅ Ancoragem de preços
- ✅ Autoridade com ícones

### Acessibilidade
- ✅ VLibras integrado
- ✅ UserWay integrado
- ✅ HTML semântico
- ✅ ARIA labels completos

