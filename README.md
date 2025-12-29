# 📰 Oxente News - Template de Jornal Online

**Portal de Notícias do Nordeste Brasileiro**  
*Informação com o tempero nordestino desde 2025*

![Status do Projeto](https://img.shields.io/badge/status-em%20produção-green)
![Licença](https://img.shields.io/badge/licença-MIT-blue)
![Tecnologias](https://img.shields.io/badge/tecnologias-HTML%2C%20CSS%2C%20JavaScript-yellow)
![Acessibilidade](https://img.shields.io/badge/acessibilidade-WCAG%20AA%20compatible-orange)

<div align="center">
  <img src="https://template-web-newspapper.vercel.app/" alt="Preview do Oxente News" width="600">
  <p><em>Visite o projeto online: <a href="https://template-web-newspapper.vercel.app/" target="_blank">https://template-web-newspapper.vercel.app/</a></em></p>
</div>

## ✨ Características Principais

- 🎨 **Design autêntico nordestino** com paleta de cores e tipografia regional
- 📱 **Totalmente responsivo** para mobile, tablet e desktop
- 🚀 **Performance otimizada** com carregamento rápido
- ♿ **Acessibilidade implementada** seguindo diretrizes WCAG
- 🧩 **Estrutura modular** para fácil manutenção e expansão
- 🔧 **Pronto para APIs** de clima, cotações e notícias em tempo real

## 🎯 Objetivo do Projeto

O **Oxente News** é um template estático para jornal online desenvolvido para portfólio, demonstrando habilidades em desenvolvimento front-end com código limpo, estrutura modular e preparação para integração com APIs externas. O projeto celebra a cultura nordestina brasileira através de seu design e conteúdo.

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Descrição |
|------------|-----------|
| ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white) | Estrutura semântica e acessível |
| ![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white) | Estilização moderna com Grid/Flexbox |
| ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) | Interatividade e consumo de APIs |
| ![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white) | Hospedagem e deploy contínuo |
| ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) | Controle de versão |

## 📂 Estrutura do Projeto

```
oxente-news/
│
├── 📁 assets/                 # Recursos estáticos
│   ├── 📁 css/               # Folhas de estilo
│   │   ├── main.css          # Estilos principais
│   │   ├── responsive.css    # Media queries
│   │   └── variables.css     # Variáveis CSS (cores, fontes)
│   │
│   ├── 📁 js/                # Scripts JavaScript
│   │   ├── main.js           # Lógica principal
│   │   ├── api-integration.js # Integração com APIs
│   │   └── components.js     # Componentes reutilizáveis
│   │
│   └── 📁 images/            # Imagens e ícones
│       ├── 📁 backgrounds/   # Imagens de fundo
│       ├── 📁 icons/         # Ícones do sistema
│       └── 📁 logos/         # Logotipos e marcas
│
├── 📁 components/            # Componentes reutilizáveis
│   ├── header.html           # Cabeçalho da aplicação
│   ├── footer.html           # Rodapé da aplicação
│   ├── news-card.html        # Card de notícia
│   ├── sidebar-widget.html   # Widget lateral
│   └── modal.html            # Modal para imagens
│
├── 📁 pages/                 # Páginas do site
│   ├── index.html            # Página inicial
│   ├── news/                 # Página de notícias
│   ├── categories/           # Página por categorias
│   └── about.html            # Sobre o projeto
│
├── 📁 api/                   # Configurações de APIs
│   ├── weather.config.js     # Configuração de clima
│   ├── currency.config.js    # Configuração de cotações
│   └── news.config.js        # Configuração de notícias
│
├── 📄 index.html             # Página principal
├── 📄 README.md              # Documentação do projeto
├── 📄 package.json           # Dependências do projeto
└── 📄 vercel.json            # Configuração do Vercel
```

## 🚀 Como Executar o Projeto

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/oxente-news.git
cd oxente-news
```

### 2. Execute localmente
Como é um projeto estático, basta abrir o arquivo `index.html` em seu navegador ou usar um servidor local:

```bash
# Com Python
python -m http.server 8000

# Com Node.js (instale o http-server primeiro)
npx http-server
```

### 3. Acesse no navegador
Abra [http://localhost:8000](http://localhost:8000) ou a porta configurada.

## 🔧 Configuração de APIs

O projeto está preparado para integrar com as seguintes APIs:

### 🌤️ API de Clima (OpenWeatherMap)
```javascript
// api/weather.config.js
const weatherConfig = {
  apiKey: 'SUA_CHAVE_API_AQUI',
  cities: ['Recife', 'Salvador', 'Fortaleza', 'Natal'],
  units: 'metric',
  language: 'pt_br'
};
```

### 💱 API de Cotações (ExchangeRate-API)
```javascript
// api/currency.config.js
const currencyConfig = {
  apiKey: 'SUA_CHAVE_API_AQUI',
  baseCurrency: 'BRL',
  targetCurrencies: ['USD', 'EUR', 'GBP'],
  updateInterval: 3600000 // 1 hora
};
```

### 📰 API de Notícias (NewsAPI)
```javascript
// api/news.config.js
const newsConfig = {
  apiKey: 'SUA_CHAVE_API_AQUI',
  country: 'br',
  category: 'general',
  pageSize: 10
};
```

## 🎨 Design System

### Paleta de Cores
```css
:root {
  --primary: #2E8B57;      /* Verde Sertão */
  --secondary: #FF8C00;    /* Laranja do Sol Nordestino */
  --accent: #8B4513;       /* Marrom da Terra */
  --light: #F5F5DC;        /* Bege Clareio */
  --dark: #2F4F4F;         /* Azul Petróleo */
  --text: #333333;         /* Texto principal */
  --background: #FFFFFF;    /* Fundo */
}
```

### Tipografia
- **Títulos:** 'Montserrat' (importância e modernidade)
- **Corpo do texto:** 'Open Sans' (legibilidade otimizada)
- **Ênfases e destaques:** 'Roboto Slab' (personalidade)


## ♿ Acessibilidade

Implementamos diversas práticas para garantir acessibilidade:

- ✅ Navegação por teclado completa
- ✅ Alto contraste (WCAG AA)
- ✅ Textos alternativos descritivos em todas as imagens
- ✅ Semântica HTML5 apropriada (`<article>`, `<section>`, `<nav>`)
- ✅ ARIA labels e roles onde necessário
- ✅ Foco visível em todos os elementos interativos



<div align="center">
  <p><strong>Oxente News</strong> - Celebrando a cultura nordestina através do jornalismo digital</p>
  <p>
    <a href="https://template-web-newspapper.vercel.app/" target="_blank">🌐 Site Oficial</a> •
    <a href="https://github.com/seu-usuario/oxente-news" target="_blank">📦 Código Fonte</a> •
    <a href="https://github.com/seu-usuario/oxente-news/issues" target="_blank">🐛 Reportar Problema</a>
  </p>
</div>

---
⭐ **Gostou do projeto?** Deixe uma estrela no repositório!  
🚀 **Quer usar em seu portfólio?** Faça um fork e adapte para suas necessidades.  
💬 **Dúvidas ou sugestões?** Abra uma issue no GitHub.
