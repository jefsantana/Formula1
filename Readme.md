# 🏎️ Fórmula 1 Racing - Portal Oficial

Um portal moderno e profissional sobre Fórmula 1, desenvolvido com HTML5, CSS3 e JavaScript vanilla.

## ✨ Características Principais

### Design Moderno
- **Interface Dark Mode** - Design elegante com tema escuro profissional
- **Animações Suaves** - Transições e animações em CSS e JavaScript
- **Efeitos 3D** - Cards com efeito de inclinação (tilt) ao passar o mouse
- **Parallax** - Efeito parallax na imagem principal do hero
- **Gradientes Dinâmicos** - Uso extensivo de gradientes modernos

### Funcionalidades

#### 🎯 Navegação
- Navbar fixo com efeito de transparência e blur
- Menu mobile responsivo com animação
- Indicador visual da seção ativa
- Smooth scroll para todas as âncoras
- Botão "voltar ao topo" animado

#### 🏁 Seções
1. **Hero Section**
   - Background com overlay e gradiente
   - Estatísticas animadas com contador
   - Call-to-actions destacados
   - Indicador de scroll

2. **Carros**
   - Grid responsivo com cards das equipes
   - Hover effects com transformação 3D
   - Badges coloridos por equipe
   - Estatísticas de vitórias e títulos

3. **Equipes**
   - Cards com logos e bandeiras
   - Destaque para equipes campeãs
   - Imagens dos carros de cada equipe
   - Informações de localização

4. **Pilotos**
   - Imagem hero com overlay
   - Grid organizado por equipe
   - Números dos pilotos
   - Cores das equipes

5. **Notícias**
   - Cards clicáveis para portais de notícias
   - Hover effects sofisticados
   - Links para os principais sites especializados

6. **Footer**
   - Múltiplas seções informativas
   - Newsletter com validação
   - Links para redes sociais
   - Navegação secundária

### 🎨 Design System

#### Cores Principais
```css
--primary: #E10600        /* Vermelho F1 */
--secondary: #15151E      /* Cinza escuro */
--dark: #0A0A0F          /* Preto */
```

#### Cores das Equipes
- Ferrari: #E80020
- Mercedes: #27F4D2
- Red Bull: #3671C6
- McLaren: #FF8000
- Alpine: #0093CC
- Aston Martin: #229971
- Williams: #64C4FF
- Haas: #B6BABD
- Sauber: #52E252
- RB: #6692FF

#### Tipografia
- **Display**: Playfair Display (títulos)
- **Corpo**: Inter (textos)

### 📱 Responsividade

O site é totalmente responsivo com breakpoints:
- Desktop: > 1024px
- Tablet: 768px - 1024px
- Mobile: < 768px
- Small Mobile: < 480px

### ⚡ Performance

#### Otimizações Implementadas
- Lazy loading de imagens
- Debounce em eventos de scroll
- IntersectionObserver para animações
- Preload de imagens críticas
- CSS otimizado com variáveis
- JavaScript modular e organizado

### 🎭 Animações

1. **Fade In Up** - Elementos aparecem de baixo para cima
2. **Tilt Effect** - Cards inclinam em 3D no hover
3. **Scale** - Imagens crescem ao passar o mouse
4. **Parallax** - Movimento de parallax no background
5. **Counter** - Contadores animados de estatísticas
6. **Stagger** - Animações escalonadas em grids

### 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **CSS3** - Estilização moderna com:
  - Variáveis CSS (Custom Properties)
  - Flexbox e Grid Layout
  - Animations e Transitions
  - Backdrop Filters
  - Gradients
- **JavaScript (ES6+)** - Interatividade com:
  - IntersectionObserver API
  - Event Delegation
  - Debouncing
  - Módulos
- **Font Awesome 6** - Ícones
- **Google Fonts** - Fontes (Playfair Display, Inter)

### 📂 Estrutura de Arquivos

```
projeto/
│
├── index.html          # Estrutura HTML principal
├── styles.css          # Estilos CSS
├── script.js           # JavaScript
│
└── assets/             # Pasta de recursos
    ├── logo.png
    ├── img4.jpg        # Hero background
    ├── pilotos.jpg
    ├── carros/         # Imagens dos carros
    ├── logos/          # Logos das equipes
    ├── bandeiras/      # Bandeiras dos países
    └── noticias/       # Logos dos portais
```

### 🚀 Como Usar

1. **Clone o repositório**
```bash
git clone https://github.com/seu-usuario/f1-racing.git
cd f1-racing
```

2. **Abra o arquivo**
```bash
# Simplesmente abra o index.html em um navegador
# Ou use um servidor local:
python -m http.server 8000
# ou
npx serve
```

3. **Acesse**
```
http://localhost:8000
```

### 🎨 Customização

#### Alterar Cores
Edite as variáveis CSS em `styles.css`:
```css
:root {
    --primary: #SUA_COR;
    --secondary: #SUA_COR;
    /* ... */
}
```

#### Adicionar Nova Equipe
1. Adicione as imagens em `/assets`
2. Copie um card existente no HTML
3. Ajuste as informações
4. A responsividade será automática

#### Modificar Animações
Ajuste as propriedades de transição:
```css
.elemento {
    transition: transform 0.3s ease;
}
```

### 🔧 Funcionalidades JavaScript

#### Navbar Scroll
```javascript
window.addEventListener('scroll', () => {
    if (window.scrollY > 100) {
        navbar.classList.add('scrolled');
    }
});
```

#### Animação de Contadores
```javascript
function animateCounter(element, target, duration) {
    // Anima números de 0 até o valor alvo
}
```

#### IntersectionObserver
```javascript
const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.style.opacity = '1';
        }
    });
});
```

### 📊 Seções Futuras (Roadmap)

- [ ] Sistema de busca de pilotos/equipes
- [ ] Calendário interativo de corridas
- [ ] Tabela de classificação ao vivo
- [ ] Galeria de fotos
- [ ] Vídeos highlights
- [ ] Comparador de pilotos
- [ ] Quiz sobre F1
- [ ] Modo claro/escuro toggle
- [ ] Múltiplos idiomas

### 🐛 Bugs Conhecidos

Nenhum bug conhecido no momento. Reporte issues em:
https://github.com/seu-usuario/f1-racing/issues

### 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

### 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

### 👨‍💻 Autor

**Seu Nome**
- GitHub: [@seu-usuario](https://github.com/seu-usuario)
- LinkedIn: [Seu Perfil](https://linkedin.com/in/seu-perfil)
- Email: seu.email@example.com

### 🙏 Agradecimentos

- Fórmula 1 pela inspiração
- Comunidade de desenvolvedores
- Font Awesome pelos ícones
- Google Fonts pelas fontes

### 📸 Screenshots

#### Desktop
![Desktop Hero](screenshots/desktop-hero.png)
![Desktop Grid](screenshots/desktop-grid.png)

#### Mobile
![Mobile Hero](screenshots/mobile-hero.png)
![Mobile Menu](screenshots/mobile-menu.png)

### 🌐 Browser Support

- Chrome (últimas 2 versões)
- Firefox (últimas 2 versões)
- Safari (últimas 2 versões)
- Edge (últimas 2 versões)

### 📞 Suporte

Para suporte, envie um email para suporte@f1racing.com ou abra uma issue no GitHub.

---

**⚡ Desenvolvido com paixão pela Fórmula 1 e tecnologia web moderna**