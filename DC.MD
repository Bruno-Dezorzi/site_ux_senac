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
- **Header (linha 36)**: Logo, contatos e busca agrupados
- **Contact Info (linha 84)**: Links de contato agrupados com `gap: 20px`
- **Vehicle Info (linha 457)**: Título, detalhes e preço juntos no card

### 🔹 ALINHAMENTO
Nada deve ser colocado arbitrariamente.

**Aplicações:**
- **Navigation (linha 160)**: Menu centralizado com `justify-content: center`
- **Hero Content (linha 228)**: Conteúdo centralizado vertical e horizontalmente
- **Section Titles (linha 310)**: Títulos centralizados

### 🔹 REPETIÇÃO
Repetir elementos visuais em todo o material.

**Aplicações:**
- **Links (linha 95)**: Padrão consistente para todos os links do header
- **Cards (linha 349)**: Todos os cards de veículos seguem o mesmo padrão
- **Buttons (linha 501)**: CTAs com o mesmo estilo de gradiente

### 🔹 CONTRASTE
Fazer elementos diferentes realmente diferentes.

**Aplicações:**
- **Logo (linha 49)**: Branco sobre gradiente roxo
- **Search Button (linha 139)**: Laranja destacado `#f39c12`
- **Vehicle Price (linha 485)**: Preço em roxo grande `font-size: 24px`

---

## 2. Leis do Design

### 🔹 LEI DE FITTS
Alvos maiores e mais próximos são mais fáceis de acertar.

**Aplicações:**
- **Botões (linha 95)**: `padding: 6px 12px` para área clicável adequada
- **Navigation (linha 172)**: `padding: 18px 25px` em links de menu
- **Mobile (linha 768)**: Botões ainda maiores no mobile

### 🔹 LEI DE HICK
Mais opções = mais tempo de decisão.

**Aplicações:**
- **Menu (HTML)**: Apenas 6 itens no menu principal
- **Search (linha 119)**: Um único campo de busca simplificado

### 🔹 LEI DE MILLER (7±2)
Limite de 7±2 itens na memória de trabalho.

**Aplicações:**
- **Navigation**: 6 itens (Home, Estoque, Avaliação, Financiamento, Empresa, Contato)
- **Hero Stats (linha 271)**: 3 estatísticas apenas
- **Features (linha 534)**: 3 features principais

### 🔹 LEI DA GESTALT

**Similaridade (linha 349)**: Cards similares são percebidos como grupo
**Região Comum (linha 349)**: Cards com fundo branco formam unidades visuais
**Simetria (linha 330)**: Grid simétrico 4 colunas

---

## 3. Heurísticas de Nielsen

### ✅ 1. Visibilidade do Status do Sistema
- **Sticky Header (linha 36)**: `position: sticky` - sempre visível
- **Active Nav (linha 186)**: Menu ativo destacado em roxo

### ✅ 2. Correspondência com Mundo Real
- **Labels**: "Home", "Estoque", "Contato" - linguagem familiar
- **Icons**: Telefone, WhatsApp, mapa - ícones reconhecíveis

### ✅ 4. Consistência e Padrões
- **Colors**: Paleta roxo/laranja consistente em todo site
- **Transitions**: Todas em `0.3s ease`
- **Border Radius**: Todos os cards com `12px`

### ✅ 6. Reconhecimento ao Invés de Memorização
- **Icons (linha 565)**: Ícones grandes de 48px para fácil reconhecimento
- **Badge "OFERTA" (linha 376)**: Visualmente destacado

### ✅ 8. Design Estético e Minimalista
- **Cards (linha 349)**: Apenas informações essenciais
- **Layout limpo**: Muito espaço em branco

---

## 4. Vieses Cognitivos

### 🧠 PROVA SOCIAL
**Onde:** Hero Stats (linha 271)
```html
500+ Veículos Vendidos
100% Procedência
10+ Anos de Experiência
```
**Por quê:** Demonstra credibilidade e confiança

### 🧠 ESCASSEZ
**Onde:** Badge "OFERTA" (linha 376)
```css
.vehicle-badge {
  animation: pulse 2s infinite;
}
```
**Por quê:** Cria senso de urgência

### 🧠 ANCORAGEM
**Onde:** Preço antigo (linha 477)
```html
<p class="old-price">de R$ 55.900</p>
<div class="vehicle-price">R$ 53.900</div>
```
**Por quê:** Faz o preço atual parecer melhor negócio

### 🧠 AUTORIDADE
**Onde:** Feature Icons (linha 565)
```html
<i class="fas fa-shield-alt"></i>
100% Procedência
```
**Por quê:** Ícone de escudo transmite segurança e confiança

---

## 5. IHC

### 💡 FEEDBACK VISUAL
**Aplicações:**
- **Hover cards (linha 364)**: `transform: translateY(-10px)` ao passar mouse
- **Button active (linha 150)**: `transform: scale(0.98)` ao clicar
- **Input focus (linha 151)**: Outline laranja ao focar

### 💡 AFFORDANCE
Elementos que indicam como usá-los:
- **Cursor pointer (linha 106)**: Indica clicabilidade
- **Button gradients (linha 501)**: Sombras indicam que é clicável
- **Hover effects**: Mudanças visuais mostram interatividade

### 💡 ACESSIBILIDADE
- **VLibras**: Plugin para pessoas surdas (HTML)
- **UserWay**: Ferramentas de acessibilidade (HTML)
- **ARIA labels**: Em todos elementos interativos
- **Semantic HTML**: `<header>`, `<nav>`, `<section>`, `<article>`, `<footer>`
- **Loading lazy**: `<img loading="lazy">` para performance

### 💡 NAVEGAÇÃO INTUITIVA
- **Sticky nav (linha 160)**: `position: sticky` - sempre disponível
- **Smooth scroll (linha 816)**: `scroll-behavior: smooth`
- **Active state (linha 186)**: Mostra onde usuário está

---

## 📊 Resumo Quantitativo

| Categoria | Quantidade |
|-----------|------------|
| **Robin Williams** | 12 aplicações |
| **Leis do Design** | 8 aplicações |
| **Heurísticas Nielsen** | 5 aplicações |
| **Vieses Cognitivos** | 4 aplicações |
| **IHC** | 8 aplicações |
| **TOTAL** | **37 implementações** |

---

## 🎯 Principais Destaques

### Design Visual
- ✅ Paleta de cores consistente (roxo + laranja)
- ✅ Hierarquia visual clara
- ✅ Espaçamento harmônico
- ✅ Contraste adequado

### Usabilidade
- ✅ Navegação intuitiva
- ✅ Feedback em todas interações
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

---

## 📝 Conclusão

O site AutoPrime foi desenvolvido seguindo rigorosamente os principais conceitos de UX/UI Design, garantindo uma experiência de usuário otimizada, acessível e psicologicamente persuasiva. Todos os princípios foram aplicados de forma intencional e documentada, criando uma interface profissional e eficiente.

---

**Desenvolvido para trabalho acadêmico de UX/UI Design**