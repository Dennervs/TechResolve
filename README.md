# TechResolve - Site Portfolio

Este é um site portfolio desenvolvido para a TechResolve, uma empresa de tecnologia.

## Características

- **Fonte**: Roboto-BoldItalic aplicada em todo o projeto
- **Fundo**: Imagem de fundo única (img9.png.jpeg) aplicada em todo o site
- **Design**: Interface moderna com efeitos de vidro (glassmorphism)
- **Responsivo**: Adaptável a diferentes tamanhos de tela
- **Otimizado**: Configurado para funcionar sem usar o diretório diretamente

## Estrutura do Projeto

```
techresolv/
├── css/
│   ├── style.css          # Estilos principais
│   ├── fonts.css          # Configuração de fontes
│   ├── responsive.css     # Estilos responsivos
│   └── partials/          # Arquivos CSS parciais
├── js/
│   └── bootstrap.min.js   # JavaScript do Bootstrap
├── prints/                # Imagens do projeto
├── fontes/                # Arquivos de fonte
├── icons/                 # Ícones Font Awesome
├── index.html             # Página principal
├── .htaccess              # Configuração do servidor
└── README.md              # Este arquivo
```

## Como Usar

### Opção 1: Servidor Local (XAMPP/WAMP)
1. Coloque a pasta `techresolv` no diretório `htdocs` do XAMPP
2. Inicie o Apache no painel de controle do XAMPP
3. Acesse `http://localhost/techresolv` no navegador

### Opção 2: Servidor Web
1. Faça upload de todos os arquivos para o servidor web
2. O arquivo `.htaccess` configurará automaticamente as regras de reescrita
3. Acesse o domínio no navegador

## Configurações

### Fonte
- A fonte Roboto-BoldItalic está configurada em `css/fonts.css`
- Aplicada globalmente através da variável CSS `--roboto`

### Fundo
- A imagem de fundo está configurada no `body` em `css/style.css`
- Aplicada com `background-size: cover` para cobrir toda a tela
- Efeito de overlay para melhorar a legibilidade do texto

### Navegação
- O arquivo `.htaccess` remove a necessidade de usar `.html` nas URLs
- Configuração de cache e compressão para melhor performance

## Tecnologias Utilizadas

- HTML5
- CSS3 (com variáveis CSS e efeitos modernos)
- Bootstrap 5
- Font Awesome
- JavaScript

## Personalização

Para personalizar o site:

1. **Fonte**: Edite `css/fonts.css` e `css/partials/_variables.css`
2. **Cores**: Modifique as variáveis em `css/partials/_variables.css`
3. **Fundo**: Altere a imagem em `css/style.css` (linha 13)
4. **Conteúdo**: Edite `index.html`

## Suporte

Para dúvidas ou suporte, entre em contato com a equipe TechResolve.
