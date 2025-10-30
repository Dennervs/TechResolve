# Guia Bootstrap - TechResolve

Este guia explica como o Bootstrap 5.0.2 está sendo utilizado no projeto TechResolve.

## 🚀 Bootstrap 5.0.2 Implementado

### Estrutura de Arquivos
```
bootstrap-5.0.2-dist/
├── css/
│   ├── bootstrap.min.css          # CSS principal
│   ├── bootstrap.css.map          # Source map
│   └── ...                        # Outros arquivos CSS
└── js/
    ├── bootstrap.bundle.min.js    # JavaScript completo
    ├── bootstrap.bundle.js.map    # Source map
    └── ...                        # Outros arquivos JS
```

## 🎨 Componentes Bootstrap Utilizados

### 1. **Navbar (Navegação)**
- **Classe**: `navbar navbar-expand-lg navbar-dark fixed-top`
- **Recursos**:
  - Navbar fixa no topo
  - Responsiva com collapse
  - Ícones Font Awesome nos links
  - Efeitos hover personalizados

```html
<nav class="navbar navbar-expand-lg navbar-dark fixed-top">
    <div class="container">
        <a class="navbar-brand d-flex align-items-center" href="#">
            <img src="..." alt="TechResolve" height="40" class="me-2">
            <span class="fw-bold">TechResolve</span>
        </a>
        <!-- Menu responsivo -->
    </div>
</nav>
```

### 2. **Grid System**
- **Classes**: `container`, `row`, `col-*`
- **Recursos**:
  - Sistema de 12 colunas
  - Breakpoints responsivos (xs, sm, md, lg, xl, xxl)
  - Gaps personalizados com `g-4`

```html
<div class="container">
    <div class="row g-4">
        <div class="col-lg-6 col-md-12">
            <!-- Conteúdo -->
        </div>
    </div>
</div>
```

### 3. **Cards**
- **Classes**: `card`, `card-body`, `card-title`
- **Recursos**:
  - Cards da equipe com hover effects
  - Cards de tecnologias com filtros
  - Altura uniforme com `h-100`

```html
<div class="card h-100 border-0 shadow-lg team-card">
    <div class="card-body p-4 text-center">
        <!-- Conteúdo do card -->
    </div>
</div>
```

### 4. **Buttons**
- **Classes**: `btn`, `btn-primary`, `btn-outline-*`
- **Recursos**:
  - Botões com gradientes personalizados
  - Efeitos hover com transform
  - Tamanhos variados (sm, lg)
  - Ícones integrados

```html
<button type="button" class="btn btn-primary btn-lg px-4 py-3 fw-bold">
    <i class="fas fa-user me-2"></i>Sobre Mim
</button>
```

### 5. **Typography**
- **Classes**: `display-*`, `fw-bold`, `text-*`
- **Recursos**:
  - Classes de display responsivas
  - Peso de fonte personalizado
  - Cores e alinhamentos

```html
<h1 class="display-2 fw-bold text-uppercase mb-3">Eu sou Denner</h1>
<p class="lead mb-4">Descrição do desenvolvedor</p>
```

### 6. **Utilities**
- **Classes**: `d-flex`, `justify-content-*`, `align-items-*`
- **Recursos**:
  - Flexbox utilities
  - Spacing (margin/padding)
  - Text utilities
  - Display utilities

## 🎯 Recursos Avançados Implementados

### 1. **Glassmorphism Effect**
```css
.team-card {
    background: rgba(255, 255, 255, 0.95) !important;
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.2) !important;
}
```

### 2. **Hover Animations**
```css
.team-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3) !important;
}
```

### 3. **Responsive Design**
- Breakpoints personalizados
- Imagens responsivas
- Texto adaptativo
- Layout flexível

### 4. **Custom CSS Variables**
```css
:root {
    --primary-color: #854fee;
    --gradient-color: linear-gradient(90deg, #4458dc 0%, #854fee 100%);
    --roboto: 'Roboto', sans-serif;
}
```

## 📱 Responsividade

### Breakpoints Utilizados
- **xs**: < 576px (Mobile pequeno)
- **sm**: ≥ 576px (Mobile)
- **md**: ≥ 768px (Tablet)
- **lg**: ≥ 992px (Desktop)
- **xl**: ≥ 1200px (Desktop grande)
- **xxl**: ≥ 1400px (Desktop extra grande)

### Classes Responsivas
```html
<div class="col-lg-6 col-md-12 col-sm-12">
    <!-- 6 colunas em desktop, 12 em tablet e mobile -->
</div>

<div class="d-flex flex-column flex-sm-row gap-3">
    <!-- Flex column em mobile, row em tablet+ -->
</div>
```

## 🛠️ Personalizações CSS

### 1. **Override de Classes Bootstrap**
```css
.btn-primary {
    background: var(--gradient-color) !important;
    border: none !important;
    font-weight: bold;
    transition: all 0.3s ease;
}
```

### 2. **Componentes Customizados**
```css
.team-card {
    /* Estilos específicos para cards da equipe */
}

.brand-card {
    /* Estilos específicos para cards de marcas */
}
```

### 3. **Animações Personalizadas**
```css
.navbar-nav .nav-link::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 0;
    height: 2px;
    background: var(--primary-color);
    transition: all 0.3s ease;
    transform: translateX(-50%);
}
```

## 🎨 Temas e Cores

### Paleta de Cores
- **Primary**: #854fee (Roxo)
- **Gradient**: linear-gradient(90deg, #4458dc 0%, #854fee 100%)
- **Background**: Imagem com overlay
- **Text**: Branco com sombras para legibilidade

### Aplicação de Cores
```html
<!-- Texto primário -->
<h5 class="text-primary fw-bold">CEO</h5>

<!-- Botão com gradiente -->
<button class="btn btn-primary">Botão</button>

<!-- Botão outline -->
<button class="btn btn-outline-light">Botão Outline</button>
```

## 📋 Checklist de Implementação

- [x] Bootstrap 5.0.2 CSS carregado
- [x] Bootstrap 5.0.2 JS carregado
- [x] Navbar responsiva implementada
- [x] Grid system utilizado
- [x] Cards personalizados
- [x] Botões com estilos customizados
- [x] Typography responsiva
- [x] Utilities do Bootstrap
- [x] Efeitos glassmorphism
- [x] Animações hover
- [x] Design responsivo
- [x] Integração com Font Awesome
- [x] CSS customizado para override

## 🚀 Próximos Passos

1. **Adicionar mais componentes Bootstrap**:
   - Modals
   - Carousels
   - Accordions
   - Tooltips
   - Popovers

2. **Melhorar acessibilidade**:
   - ARIA labels
   - Navegação por teclado
   - Contraste de cores

3. **Otimizações**:
   - Lazy loading de imagens
   - Minificação de CSS
   - Compressão de assets

## 📚 Recursos Úteis

- [Bootstrap 5.0.2 Documentation](https://getbootstrap.com/docs/5.0/)
- [Bootstrap Icons](https://icons.getbootstrap.com/)
- [Font Awesome Icons](https://fontawesome.com/)
- [CSS Grid vs Flexbox](https://css-tricks.com/snippets/css/complete-guide-grid/)

---

**Desenvolvido com ❤️ pela equipe TechResolve**
