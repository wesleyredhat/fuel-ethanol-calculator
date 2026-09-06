# Fuel Ethanol Calculator

Calculadora de abastecimento para carros com remap E30–E85: informa quanto colocar em cada bomba (gasolina e etanol) para atingir a mistura alvo, considerando o etanol que a gasolina brasileira já contém (comum 32%, Podium 25%).

Arquivo único (`index.html`), sem dependências, funciona offline. Pensado para iPhone.

## Publicar no GitHub Pages

1. Suba estes arquivos para a raiz de um repositório público.
2. No repositório: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
3. Aguarde cerca de um minuto. A URL aparece no topo da página Pages:
   `https://SEU-USUARIO.github.io/NOME-DO-REPO/`
4. No iPhone, abra essa URL no Safari → botão Compartilhar → **Adicionar à Tela de Início**.

## Ajustes rápidos

No começo do `<script>` em `index.html`:

```js
var GAS = { comum:{pct:32}, podium:{pct:25} };   // % de etanol anidro na gasolina
```

Faixa da barra e marcas: atributos `min`/`max` do `<input type="range">` e os botões dentro de `.ticks`.
