# Meu Orçamento

Webapp de controle de receitas e despesas mensais. Funciona offline, sem servidor nem login — os dados ficam salvos no próprio navegador.

## Recursos
- **Painel** com KPIs, gráficos (evolução da conta, receitas × despesas, composição, saldo mensal) e alertas automáticos.
- **Lançar mês**: entrada rápida de receitas, despesas fixas e faturas dos cartões.
- **Recorrentes**: todos os compromissos recorrentes e os descontos em folha, editáveis.
- **Consignados**: parcelas que avançam automaticamente a cada mês, com opção de quitar.
- **Metas**: checklist de economia com acompanhamento.
- **Vários anos**: seletor de ano; o saldo final de dezembro vira o inicial de janeiro seguinte.
- **Sincronização na nuvem**: com um código secreto, os dados salvam e sincronizam entre aparelhos (Netlify Function + Netlify Blobs).
- **Backup**: exportar/importar `.json` como cópia de segurança.

## Como usar
Abra o `index.html` em qualquer navegador moderno. No celular, use "Adicionar à Tela de Início" para virar um app.

## Publicar online
Veja [COMO-HOSPEDAR.md](COMO-HOSPEDAR.md) — inclui GitHub Pages, Netlify e Vercel (todos grátis).

## Sincronização na nuvem (Netlify)
Para sincronizar entre aparelhos, o app precisa ser hospedado no **Netlify**, que roda a função `netlify/functions/sync.mjs` (usa Netlify Blobs). Em Config, defina um **código secreto** (mín. 6 caracteres) e use o mesmo em cada aparelho. O código funciona como senha — escolha algo longo e não óbvio.

## Tecnologia
Frontend: HTML, CSS e JavaScript puro (arquivo único). Gráficos com [Chart.js](https://www.chartjs.org/) via CDN.
Backend de sincronização: Netlify Function (`@netlify/blobs`).

## Privacidade
Sem sincronização, os dados ficam só no navegador. Com sincronização, ficam também nos Netlify Blobs, acessíveis apenas por quem tem o código — nunca no repositório público.
