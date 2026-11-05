# Vitrine Bentivi (NestJS)

A página fica em `public/index.html` e é servida pelo NestJS.
É a mesma página do projeto Next.js (`bentivi-orcamento/prototipo/index.html`): ajuste de layout vale para os dois.

## Rodar no computador
npm install
npm run build
npm start
Abra http://localhost:3000 (vendedor: http://localhost:3000/?v=samuel)

## Colocar no ar

### Vercel (grátis, página estática)
O `vercel.json` manda a Vercel entregar a pasta `public/` direto pela CDN, sem instalar
nem compilar nada: o NestJS não roda lá, e não precisa — a página é um HTML só.
Conectado ao GitHub, cada push no branch de produção publica sozinho.
Vendedor continua funcionando pelo endereço: `https://SEU-ENDERECO.vercel.app/?v=samuel`.

### Render, Railway ou similar (com o servidor NestJS)
- Build command: npm install && npm run build
- Start command: npm start
(a porta é lida da variável PORT)

No ar no Railway: projeto "Bentivi Vitrine", serviço com este repositório (build `npm run build`, start `npm start`).

## Alterar a página
Edite `public/index.html`, no bloco CONFIG do script:
- WhatsApp: `numeroPadrao` e `vendedores`
- Preços, textos e cardápio: `opcoes`
- Fotos: `fotos` de cada opção (só fotos reais do Bentivi)
