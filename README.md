<div align="center">

# Monte seu Lego

Monte seu próprio boneco LEGO, escolha as cores e a expressão e compartilhe o resultado.

[![Ver site](https://img.shields.io/badge/VER_SITE-0D0D0D?style=for-the-badge&logo=netlify&logoColor=FF003C)](https://monteseulego.netlify.app)

![HTML5](https://img.shields.io/badge/HTML5-0D0D0D?style=for-the-badge&logo=html5&logoColor=FF003C)
![CSS3](https://img.shields.io/badge/CSS3-0D0D0D?style=for-the-badge&logo=css&logoColor=FF003C)
![JavaScript](https://img.shields.io/badge/JavaScript-0D0D0D?style=for-the-badge&logo=javascript&logoColor=FF003C)

</div>

## Sobre

Página interativa feita só com HTML, CSS e JavaScript puro, sem frameworks. A minifigura é desenhada inteiramente em CSS (sem imagens) e pode ser personalizada por um painel de controles. Depois de montar o boneco, o usuário pode gerar uma imagem da tela e compartilhá-la direto do navegador.

> A minifigura em HTML/CSS segue um exemplo popular da comunidade front-end. A interface em português, o botão de compartilhamento e a publicação são adaptações minhas.

## Funcionalidades

- **Minifigura 100% em CSS**: cabeça, tronco, braços, mãos, cintura e pernas montados com `div`s, gradientes e transformações.
- **6 expressões faciais** (clássica, sorriso, sorriso largo, preocupada, brava e surpresa), trocadas por um controle deslizante com transição animada.
- **Cores personalizáveis** da parte de cima e da parte de baixo em HSL (tonalidade, saturação e brilho).
- **Aleatório**: sorteia expressão e cores com um clique.
- **Separar / Juntar**: afasta as peças do boneco para mostrar como ele é montado.
- **Compartilhar**: captura a tela com `html2canvas` e envia a imagem pela Web Share API; em navegadores sem suporte, o usuário recebe um aviso.

## Tecnologias

- HTML5
- CSS3 — transformações 3D, transições e `currentColor` para colorir as peças
- JavaScript (vanilla) — eventos dos controles e manipulação de estilos
- [html2canvas 1.4.1](https://html2canvas.hertzen.com/) via CDN
- [Web Share API](https://developer.mozilla.org/pt-BR/docs/Web/API/Navigator/share)
- Fonte Montserrat (Google Fonts)
- Deploy na [Netlify](https://www.netlify.com/)

## Estrutura

```
monte-seu-lego/
├── index.html   # marcação da minifigura, painel de controles e script de compartilhamento
├── style.css    # desenho da minifigura, expressões e animações
└── main.js      # lógica de cores, expressões, aleatório e separar/juntar
```

## Como rodar localmente

Não há dependências para instalar.

```bash
git clone https://github.com/Lu1sR0/monte-seu-lego.git
cd monte-seu-lego
```

Abra o `index.html` no navegador ou use a extensão **Live Server** do VS Code.

> O botão **Compartilhar** depende da Web Share API com suporte a arquivos, disponível principalmente em navegadores mobile e em páginas servidas por HTTPS (ou `localhost`).

---

<div align="center">
Desenvolvido por <a href="https://github.com/Lu1sR0">Luis Roberto</a> · <a href="https://outframe.dev">Outframe</a>
</div>
