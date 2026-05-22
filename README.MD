# 🦁 Garagem do Leão — Muay Thai Landing Page

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![Netlify](https://img.shields.io/badge/Netlify-00C8B5?style=for-the-badge&logo=netlify&logoColor=white)](https://www.netlify.com/)

Uma landing page imersiva de alta fidelidade desenvolvida para o centro de treino de Muay Thai **Garagem do Leão** (Vila Escolar, São Paulo). Este projeto rompe com a estética tradicional de páginas estáticas ao introduzir um motor de renderização 3D dinâmico baseado em scroll e uma experiência sonora integrada.

---

## 💎 Funcionalidades e Diferenciais Técnicos

### 1. Motor de Scroll 3D (Cylinder Effect)
Desenvolvido inteiramente em JavaScript Vanilla e CSS 3D Transforms. Os elementos de texto e mapa não apenas deslizam verticalmente; eles rotacionam num eixo de profundidade (`translateZ` e `rotateX`), simulando um cilindro virtual. Esta técnica proporciona uma transição suave e um forte apelo visual (UX).

### 2. Design Visual "Premium Dark"
* **Paleta Imersiva:** Cores baseadas em preto profundo (`#050505`) e bronze metálico (`#cd7f32`).
* **Camadas de Profundidade:** Utilização de imagens laterais fixas (`z-index: 0`) e marcas d'água dinâmicas como papel de parede, revelando-se suavemente à medida que a secção principal (Hero) sobe.
* **Capa Inteligente:** A imagem de capa principal funciona como um bloqueador físico para a marca d'água no início do carregamento, limpando a confusão visual inicial.

### 3. Engenharia de Áudio Inteligente (Autoplay Adaptativo)
* O site tenta iniciar a trilha sonora (`Trilha_Garagem.mp3`) de forma autónoma através de uma promessa assíncrona.
* Caso as políticas de segurança do navegador bloqueiem a reprodução automática sem interação prévia (autoplay policy), o código trata o erro silenciosamente sem quebrar a execução do site.
* Um botão flutuante e transparente de áudio surge dinamicamente no ecrã após 250px de scroll (ou fixa-se de forma permanente em telemóveis) com animações de "pulso" e ondas sonoras em bronze para permitir o controlo manual do utilizador.

### 4. Responsividade e Performance
* **Telemóvel:** O comportamento da imagem de capa muda de `cover` para `contain` e o tamanho da marca d'água expande-se para `130vw` em dispositivos móveis, garantindo proximidade e enquadramento ideal.
* **SVG Inline de Alta Fidelidade:** A marca d'água do leão foi desenhada usando caminhos vetoriais (SVG inline), garantindo nitidez cristalina em ecrãs Retina e 4K com impacto zero no tempo de carregamento da página.
* **SEO Integrado:** Tags estruturadas no cabeçalho prontas para otimização de pesquisas locais no Google.

---

## 📂 Estrutura de Ficheiros do Projeto


```text
├── index.html                # Ficheiro principal de código (HTML, Tailwind & JS)
├── README.md                 # Documentação do projeto (este ficheiro)
└── assets/                   # Pasta para os recursos de média (opcional)
    ├── Logo_Circular.png         # Logo circular da marca (usado no Favicon)
    ├── Capa_site.jpg             # Imagem de capa (Hero) em ecrã inteiro
    ├── Lateral_esquerda_site.jpg # Silhueta lateral esquerda do lutador
    ├── Lateral_Direita_site.jpg  # Silhueta lateral direita do lutador
    └── Trilha_Garagem.mp3        # Trilha sonora ambiente (Muay Thai rhythm)

🦁 Créditos
CT Garagem do Leão.

Estudo de Caso & Desenvolvimento: Criado como um projeto de portefólio.
---

## Visite o site: https://garagem-do-leao.netlify.app/
