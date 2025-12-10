# SyntaxWear - E-commerce de Tênis e Sneakers Online

![SyntaxWear](./images/logo/logo.svg)

**SyntaxWear** é um site de e-commerce moderno e responsivo especializado em venda de tênis e sneakers de alta qualidade. O projeto foi desenvolvido com **HTML5**, **CSS3** e segue as melhores práticas de desenvolvimento web, incluindo design responsivo e acessibilidade.

## ✨ Features

- **Design Responsivo**: Otimizado para desktop, tablet e mobile
- **Header Fixo**: Navegação fixa com menu mobile burger
- **Seção Hero**: Banner principal com call-to-action atrativo
- **Categorias de Produtos**: Grid de categorias (Casual, Esporte, Moderno, Futurista)
- **Grid de Produtos**: Destaque de produtos em layout flexível
- **Footer Interativo**: Links navegáveis, formulário de newsletter e redes sociais
- **Acessibilidade**: Semântica HTML apropriada e navegação por teclado
- **Tipografia Moderna**: Font Ubuntu do Google Fonts
- **Paleta de Cores**: Design elegante com destaque em roxo (#6329A2)

---

## 📂 Estrutura do Projeto

```
ecommerce-syntaxwear/
├── index.html                 # Arquivo HTML principal
├── README.md                  # Este arquivo
├── css/                       # Estilos CSS
│   ├── reset.css             # Reset de estilos padrão do navegador
│   ├── variables.css         # Variáveis CSS (fontes, cores)
│   ├── base.css              # Estilos base (body, buttons, layout geral)
│   ├── layout.css            # Layout geral do site (não listado, referenciado)
│   └── components/           # Componentes específicos
│       ├── header.css        # Estilos do cabeçalho e navegação
│       ├── hero.css          # Estilos da seção hero/banner
│       ├── footer.css        # Estilos do rodapé
│       ├── product-category.css   # Estilos das categorias de produtos
│       └── product-grid.css  # Estilos da grid de produtos
├── images/                    # Imagens e assets
│   ├── banners/              # Banners (hero.jpg, hero-mobile.jpg, etc.)
│   ├── favicons/             # Ícones do navegador
│   ├── icons/                # Ícones SVG (user, help, bag, redes sociais)
│   ├── logo/                 # Logo do site (logo.svg)
│   └── products/             # Imagens dos produtos
├── js/                        # Pasta para JavaScript (vazia, pronta para expansão)
└── .git/                      # Repositório Git

```

---

## 🚀 Instalação e Setup

### Pré-requisitos

- Um navegador web moderno (Chrome, Firefox, Safari, Edge)
- Editor de código (VS Code, Sublime Text, etc.)
- Git (opcional, para clonar o repositório)

### Passos de Instalação

1. **Clone o repositório** (ou baixe o ZIP):
   ```bash
   git clone https://github.com/Carlos-Daniel-Rabelo/ecommerce-syntaxwear.git
   ```

2. **Abra o projeto** no seu editor de código favorito:
   ```bash
   code .  # Se usar VS Code
   ```

3. **Servir o arquivo localmente** (recomendado):
   - Use uma extensão como **Live Server** no VS Code, ou
   - Execute um servidor HTTP simples:

4. **Abra no navegador**:
   - Acesse `http://localhost:8000` (ou a porta configurada)

## 💻 Uso

### Estrutura HTML

O arquivo `index.html` contém:

- **Header**: Logo, navegação principal, links de acesso rápido e ícones (usuário, ajuda, carrinho)
- **Main Content**:
  - Seção Hero com banner e CTAs
  - Grid de Categorias (4 categorias principais)
  - Grid de Produtos com destaque principal
- **Footer**: Links de categoria, formulário de newsletter, ícones de redes sociais

### Customização

#### Alterar Cores

Edite `css/variables.css` para mudar a paleta de cores. Atualmente:
- Cor primária: `#6329A2` (roxo)
- Cor secundária: `#333333` (cinza escuro)
- Branco: `#ffffff`

#### Alterar Tipografia

A fonte padrão é **Ubuntu** (importada do Google Fonts em `variables.css`). Para mudar:

```css
/* Em variables.css */
:root {
    --fonte-principal: 'Sua Nova Fonte', sans-serif;
}
```

#### Adicionar Novos Componentes

1. Crie um novo arquivo em `css/components/` (ex: `novo-componente.css`)
2. Importe em `index.html`:
   ```html
   <link rel="stylesheet" href="./css/components/novo-componente.css">
   ```
3. Adicione a classe correspondente no HTML

---

## 🛠️ Tecnologias

### Frontend

| Tecnologia | Versão | Descrição |
|-----------|--------|-----------|
| HTML5 | - | Estrutura semântica |
| CSS3 | - | Estilos responsivos (Flexbox, Grid) |
| Google Fonts | - | Tipografia (Ubuntu) |

### Ferramentas

- **Git**: Controle de versão
- **VS Code**: Editor de código
- **Live Server**: Servidor de desenvolvimento (extensão VS Code)

---

## 📐 Convenções e Boas Práticas

### Unidades de Medida

- **`rem`**: Usado para espaçamentos, fontes e dimensões (escala com a fonte raiz, 1rem = 16px)
- **`px`**: Utilizado apenas em bordas finas, icones e casos específicos de pixel-perfect
- **`vw/vh`**: Usado em layouts responsivos quando necessário

**Exemplo**:
```css
.elemento {
    padding: 1.25rem;  /* 20px em rem */
    font-size: 1rem;   /* 16px em rem */
    border: 1px solid; /* px aceitável para bordas */
}
```

### Nomenclatura CSS

Utiliza-se **BEM-like** (Block Element Modifier) para clareza:

```css
.footer-item        /* Block */
.footer-nav ul      /* Elemento dentro de um bloco */
.btn-filled         /* Modificador */
```

### Responsividade

Breakpoints principais:
- **Desktop**: 1280px+
- **Tablet/Mobile**: até 1280px
- **Mobile pequeno**: até 768px

```css
@media (max-width: 1280px) {
    /* Estilos para tablets e mobile */
}

@media (max-width: 768px) {
    /* Estilos para mobile pequeno */
}
```

### Acessibilidade

- Semântica HTML apropriada (`<header>`, `<nav>`, `<main>`, `<footer>`)
- Atributos `aria-label` em links sem texto
- Contraste de cor apropriado
- Menu responsivo com navegação por teclado

---

## 🎯 Roadmap

### Curto Prazo (v1.0)
- [x] Layout base responsivo
- [x] Header com navegação fixa
- [x] Seção hero com banners
- [x] Grid de categorias
- [x] Grid de produtos
- [x] Footer com links e newsletter
- [ ] Adicionar JavaScript para interatividade (menu mobile burger)
- [ ] Otimizar imagens para web

### Médio Prazo (v1.5)
- [ ] Integrar carrinho de compras funcional
- [ ] Página de detalhe do produto
- [ ] Sistema de filtros e busca
- [ ] Página de checkout
- [ ] Sistema de autenticação (login/registro)

### Longo Prazo (v2.0+)
- [ ] Backend API (Node.js/Express ou similar)
- [ ] Banco de dados (MongoDB, PostgreSQL)
- [ ] Sistema de pagamento (Stripe, PayPal)
- [ ] Dashboard administrativo
- [ ] Email marketing integration
- [ ] Analytics e tracking

---

## 🤝 Contribuição

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -am 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

### Padrões de Código

- Use nomes descritivos para classes e IDs
- Mantenha a indentação em 4 espaços ou use tabs consistentemente
- Escreva comentários para lógica complexa
- Prefira unidades `rem` para espaçamentos
- Teste em múltiplos navegadores e resoluções

---

## 📱 Suporte para Navegadores

| Navegador | Versão Mínima |
|-----------|---------------|
| Chrome    | 90+           |
| Firefox   | 88+           |
| Safari    | 14+           |
| Edge      | 90+           |

---

## 📞 Contato e Suporte

- **Email**: [Seu Email]
- **GitHub Issues**: [Reportar bugs](https://github.com/Carlos-Daniel-Rabelo/ecommerce-syntaxwear/issues)
- **Redes Sociais**: Siga os links no footer do site

---

## 📄 Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

---

## 🎨 Créditos

- **Designer/Desenvolvedor**: Carlos Daniel Rabelo
- **Fontes**: Google Fonts (Ubuntu)
- **Inspiração**: Tendências modernas de e-commerce

---

## 🚀 Deploy

### Deploy no GitHub Pages

```bash
# Acesse as configurações do repositório
# Vá para Settings > Pages
# Selecione 'main' branch como source
# Seu site estará disponível em: https://Carlos-Daniel-Rabelo.github.io/ecommerce-syntaxwear
```

### Deploy em Hosting Tradicional

1. Upload via FTP para seu servidor
2. Certifique-se de que o `index.html` está na raiz
3. Acesse seu domínio

---

**Última atualização**: 10 de dezembro de 2025