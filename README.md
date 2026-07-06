# Meu Orçamento

Webapp de controle de receitas e despesas mensais. Funciona offline, sem servidor nem login — os dados ficam salvos no próprio navegador.

## Recursos
- **Painel** com KPIs, gráficos (evolução da conta, receitas × despesas, composição, saldo mensal) e alertas automáticos.
- **Lançar mês**: entrada rápida de receitas, despesas fixas e faturas dos cartões.
- **Recorrentes**: todos os compromissos recorrentes e os descontos em folha, editáveis.
- **Consignados**: parcelas que avançam automaticamente a cada mês, com opção de quitar.
- **Metas**: checklist de economia com acompanhamento.
- **Vários anos**: seletor de ano; o saldo final de dezembro vira o inicial de janeiro seguinte.
- **Backup**: exportar/importar `.json` para mover entre aparelhos.

## Como usar
Abra o `index.html` em qualquer navegador moderno. No celular, use "Adicionar à Tela de Início" para virar um app.

## Publicar online
Veja [COMO-HOSPEDAR.md](COMO-HOSPEDAR.md) — inclui GitHub Pages, Netlify e Vercel (todos grátis).

## Tecnologia
HTML, CSS e JavaScript puro, arquivo único. Único externo: [Chart.js](https://www.chartjs.org/) via CDN.

## Privacidade
Nada é enviado para servidores. Os dados ficam apenas no seu navegador e no backup que você baixar.
