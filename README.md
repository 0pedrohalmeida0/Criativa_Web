# 🚀 Agência Criativa Web - Website Responsivo

Um website moderno e profissional para uma agência de design digital, desenvolvido com HTML5, CSS3, Flexbox, CSS Grid e design responsivo.

## 📋 Visão Geral do Projeto

O site da **Agência Criativa Web** é uma aplicação web moderna, totalmente responsiva e otimizada que apresenta os serviços de uma agência de design digital. O projeto foi desenvolvido seguindo as melhores práticas de Web Design e implementa conceitos avançados de CSS.

## ✨ Recursos Implementados

### 1. **Estrutura HTML5 Semântica**
- Documento HTML5 com estrutura completa e acessível
- Uso de tags semânticas: `<header>`, `<nav>`, `<section>`, `<footer>`
- Meta tags de viewport para responsividade
- Links para Font Awesome para ícones

### 2. **Sistema de Navegação Responsivo**
- Menu Flexbox com navegação horizontal em desktop
- **Hambúrguer Menu** dinâmico que aparece em dispositivos móveis
- Animação suave do menu com transições CSS
- Links com efeito hover (underline animado)
- Menu fixo no topo com sticky positioning

### 3. **Layout com Flexbox**
- Menu de navegação utiliza `display: flex` para alinhamento horizontal
- Cabeçalho com flex layout para logo + menu + hambúrguer
- Flexbox em várias seções para alinhamento de elementos
- Seção Home com flex layout lado a lado (desktop) ou coluna (mobile)

### 4. **Layout com CSS Grid**
- **Seção Serviços**: Grid com `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr))`
  - Responsivo: 1 coluna em mobile, 2 em tablet, 3 em desktop
  - Auto-fit permite número dinâmico de colunas
  
- **Seção Depoimentos**: Grid similar para layout de cards
- **Footer**: Grid com `repeat(auto-fit, minmax(250px, 1fr))`

### 5. **Unidades Relativas e Responsivas**
Implementação extensiva de unidades relativas:

#### **Unidades Utilizadas:**
- `rem` - Para fonte, espaçamentos e tamanhos (baseado em 16px)
- `em` - Para espaçamentos relativos ao font-size local
- `%` - Para largura de containers e elementos
- `vw` - Para width baseado em viewport (banners)
- `vh` - Para altura baseado em viewport (seções)
- `fr` - Em CSS Grid para divisão de colunas

#### **Exemplo de Variáveis de Espaçamento:**
```css
--espacamento-xs: 0.25rem;
--espacamento-sm: 0.5rem;
--espacamento-md: 1rem;
--espacamento-lg: 1.5rem;
--espacamento-xl: 2rem;
--espacamento-2xl: 3rem;
--espacamento-3xl: 4rem;
```

### 6. **Design Responsivo - Media Queries**

#### **Breakpoints Implementados:**
```css
Desktop: 1024px+
Tablet: 768px até 1024px
Mobile: até 768px
Extra pequeno: até 480px
```

#### **Adaptações Responsivas:**

**Mobile (até 480px):**
- Font size reduzido para 14px
- Menu hambúrguer obrigatório
- Layout single column para todas as seções
- Espaçamentos reduzidos
- Botões com width 100%

**Tablet (768px):**
- Menu hambúrguer ativo
- Flexbox layouts como single column
- Seções adaptadas lado a lado quando possível
- Grid com 1 coluna para cards

**Desktop (1024px+):**
- Layout full com múltiplas colunas
- CSS Grid com 3 colunas para serviços
- Flexbox layouts horizontais
- Imagens otimizadas com tamanho máximo

### 7. **Imagens Responsivas**
- Uso de `<picture>` para múltiplas resoluções
- Implementação de `srcset` para diferentes tamanhos
- Atributo `alt` em todas as imagens
- `object-fit: cover` para manter proporções
- Imagens do Unsplash otimizadas para web

### 8. **Identidade Visual Moderna**

#### **Paleta de Cores:**
```css
Primária: #6366f1 (Roxo/Índigo)
Secundária: #8b5cf6 (Roxo mais escuro)
Destaque: #ec4899 (Rosa vibrante)
Sucesso: #10b981 (Verde)
Fundo: #ffffff e #f9fafb
Texto: #1f2937 e #6b7280
```

#### **Tipografia:**
- Font family: Segoe UI, Tahoma, Geneva, Verdana, sans-serif
- Font sizing com `clamp()` para responsividade fluida
- Exemplo: `font-size: clamp(2rem, 8vw, 3.5rem)`

### 9. **Seções do Website**

#### **Home - Banner de Boas-vindas**
- Fundo com gradiente linear
- Título grande e chamativo
- Subtítulo descritivo
- Botão de CTA (Call To Action)
- Imagem flutuante com animação
- Layout flex responsivo

#### **Sobre Nós**
- Descrição da agência
- Lista de valores com ícones
- Imagem lado a lado com texto
- Background color alternativo

#### **Serviços** ⭐
- Grid responsivo com 6 cards
- Ícones com gradiente de cor
- Lista de features com checkmarks
- Hover effects com elevation (translateY)
- Cards adaptáveis a qualquer tamanho de tela

#### **Depoimentos**
- Grid responsivo com 3 cards
- Fundo com gradiente
- Cards semi-transparentes com backdrop-filter
- Avaliação com estrelas
- Fotos de perfil dos clientes
- Nome e cargo do depoente

#### **Contato** 📧
- Duas colunas: informações + formulário
- Informações com ícones circulares coloridos
- Links funcionais (tel: e mailto:)
- Redes sociais com hover effects
- Formulário completo com validação básica

#### **Formulário de Contato**
- Campos: Nome, E-mail, Telefone, Assunto, Mensagem
- Select com opções de assunto
- Textarea redimensionável
- Validação HTML5 (required)
- Botão de envio com hover effects
- Mensagem informativa

#### **Footer**
- Grid com 3 colunas de conteúdo
- Links para navegação rápida
- Informações da empresa
- Copyright e direitos reservados

### 10. **Interatividade e Animações**

#### **Animações CSS:**
```css
- Menu hambúrguer com rotação dos spans
- Cards com translateY no hover
- Links com underline animado
- Imagem flutuante com keyframes
- Transições suaves em botões (0.3s)
```

#### **Efeitos Hover:**
- Botões com transformação e sombra aumentada
- Cards com elevação (translateY)
- Links com mudança de cor
- Ícones com escala (scale)

#### **JavaScript Funcional:**
- Menu hambúrguer toggle com classe `.active`
- Fechar menu ao clicar em link
- Validação básica de formulário
- Mensagem de sucesso ao enviar

### 11. **Acessibilidade**
- Atributos `aria-label` em ícones
- Atributos `alt` em imagens
- Contraste de cores adequado
- Links com texto descritivo
- Suporte a dark mode com `prefers-color-scheme`
- Suporte a movimento reduzido com `prefers-reduced-motion`

### 12. **Performance e Otimizações**
- CSS externo (separado do HTML)
- Variáveis CSS para reutilização
- Fontes do sistema (nenhuma fonte externa)
- Ícones do Font Awesome via CDN
- Imagens otimizadas do Unsplash
- `box-sizing: border-box` global
- `scroll-behavior: smooth` para navegação

### 13. **Print Styles**
- Oculta header, footer e botões
- Evita quebras de página dentro de seções
- Otimizado para impressão

## 📱 Responsividade - Breakpoints

```
┌─────────────────────────────────────────┐
│          EXTRA PEQUENO (< 480px)        │
│  - Single column layout                  │
│  - Hambúrguer menu obrigatório          │
│  - Font size 14px                       │
└─────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│    PEQUENO/MOBILE (480px - 768px)       │
│  - Single column primary                │
│  - Hambúrguer menu                      │
│  - Grid com 1 coluna                    │
└─────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│    TABLET (768px - 1024px)              │
│  - 2 colunas em alguns layouts          │
│  - Hambúrguer menu                      │
│  - Menu responsivo                      │
└─────────────────────────────────────────┘

┌─────────────────────────────────────────┐
│     DESKTOP (1024px+)                   │
│  - Menu horizontal completo             │
│  - 3 colunas em serviços                │
│  - 2 colunas em contato                 │
│  - Layout otimizado                     │
└─────────────────────────────────────────┘
```

## 🎨 Técnicas CSS Avançadas Utilizadas

### **1. CSS Variables (Custom Properties)**
```css
:root {
  --cor-primaria: #6366f1;
  --espacamento-md: 1rem;
  /* ... mais 20+ variáveis */
}
```

### **2. CSS Grid Auto-Fit**
```css
display: grid;
grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
gap: 2rem;
```

### **3. Clamp() para Font Sizing Fluído**
```css
font-size: clamp(2rem, 8vw, 3.5rem);
```

### **4. Backdrop Filter**
```css
backdrop-filter: blur(10px);
background-color: rgba(255, 255, 255, 0.1);
```

### **5. Linear Gradient**
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### **6. Keyframe Animations**
```css
@keyframes flutuando {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-20px); }
}
```

## 📦 Estrutura de Arquivos

```
Agencia_design/
├── index.html          # Arquivo HTML principal
├── estilos.css        # Arquivo CSS completo (1000+ linhas)
└── README.md          # Este arquivo
```

## 🚀 Como Usar

1. **Abrir o arquivo HTML:**
   - Abra `index.html` em qualquer navegador moderno

2. **Testar Responsividade:**
   - Use DevTools (F12) > Toggle Device Toolbar (Ctrl+Shift+M)
   - Teste em diferentes tamanhos de tela

3. **Personalizar:**
   - Modifique as variáveis CSS em `:root` para mudar cores
   - Edite o conteúdo HTML conforme necessário
   - Adicione suas imagens em lugar das do Unsplash

## 🌐 Navegadores Suportados

- Chrome/Edge (Versão 88+)
- Firefox (Versão 85+)
- Safari (Versão 14+)
- Mobile browsers (iOS Safari, Chrome Mobile)

## ✅ Requisitos Atendidos

- ✅ HTML5 estruturado e semântico
- ✅ Cabeçalho com logo e menu responsivo
- ✅ 5 Seções principais (Home, Sobre, Serviços, Depoimentos, Contato)
- ✅ Flexbox para navegação e layouts
- ✅ CSS Grid para seção de serviços
- ✅ Unidades relativas (%, vh, vw, rem, em, fr)
- ✅ Menu hambúrguer responsivo
- ✅ Imagens responsivas com srcset
- ✅ Media queries para diferentes resoluções
- ✅ Formulário de contato completo
- ✅ Design moderno e profissional
- ✅ Totalmente responsivo

## 💡 Dicas de Personalização

### Mudar cores:
```css
:root {
  --cor-primaria: SEU-HEXCOLOR;
  --cor-destaque: SEU-HEXCOLOR;
}
```

### Mudar fontes:
```css
--fonte-principal: 'Sua Fonte', sans-serif;
```

### Adicionar mais serviços:
- Copie um `.servico-card` na seção Serviços
- O grid se adaptará automaticamente

### Modificar layout em mobile:
- Edite os valores nos media queries
- Ajuste espaçamentos conforme necessário

## 📚 Conceitos Aprendidos

- ✅ Design Responsivo com Mobile First
- ✅ Flexbox vs CSS Grid
- ✅ Unidades Relativas e Fluídas
- ✅ Media Queries e Breakpoints
- ✅ CSS Variables para Manutenção
- ✅ Imagens Responsivas com Picture/Srcset
- ✅ Acessibilidade Web
- ✅ Animações e Transições CSS
- ✅ JavaScript para Interatividade
- ✅ Best Practices de Web Design

---

**Desenvolvido com ❤️ para EBAC**  
Projeto: Agência de Design Digital Responsiva  
Data: 2026
