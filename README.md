# Vitrine Bentivi (NestJS)

A página fica em `public/index.html` e é servida pelo NestJS.
É a mesma página do projeto Next.js (`bentivi-orcamento/prototipo/index.html`): ajuste de layout vale para os dois.

## Rodar no computador
npm install
npm run build
npm start
Abra http://localhost:3000 (vendedor: http://localhost:3000/?v=samuel)

## Colocar no ar
Em Render, Railway ou similar:
- Build command: npm install && npm run build
- Start command: npm start
(a porta é lida da variável PORT)

## Alterar a página
Edite `public/index.html`, no bloco CONFIG do script:
- WhatsApp: `numeroPadrao` e `vendedores`
- Preços, textos e cardápio: `opcoes`
- Fotos: `fotos` de cada opção (só fotos reais do Bentivi)
