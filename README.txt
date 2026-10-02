MAX REALMS 33 — PC + MOBILE FIX

Correção da base 32.

Problema encontrado:
- A função de redimensionamento usava `screen.getBoundingClientRect()`.
- `screen` era o objeto global do navegador, não a tela do jogo.
- Isso gerava erro JavaScript e impedia a inicialização.

Correções:
- usa agora `#gameScreen.getBoundingClientRect()`;
- funciona em PC e celular;
- mantém controles por teclado no PC e swipe no celular;
- fluxo de reinício/resultado mais robusto;
- mensagem clara se Three.js não carregar;
- LICENSE proprietária incluída.

Observação:
- Three.js é carregado pelo CDN jsDelivr, então a página precisa de internet para iniciar o motor 3D.
