# Como usar e hospedar o app

O app é a pasta **orcamento-app** (arquivos `index.html`, `manifest.json`). Não precisa de servidor, banco de dados nem login. Os dados ficam salvos no próprio navegador.

## 1. Usar agora no computador
Dê dois cliques em `index.html`. Abre no navegador e já vem com seus dados de 2026.

## 2. Usar no celular como um app
Depois de publicar online (passo 3), abra o endereço no celular e:
- **iPhone (Safari):** botão Compartilhar → *Adicionar à Tela de Início*.
- **Android (Chrome):** menu ⋮ → *Adicionar à tela inicial*.

Vira um ícone de app, abre em tela cheia.

## 3. Publicar online de graça (acesso de qualquer lugar)

Escolha **uma** opção. Todas são gratuitas.

### Opção A — Netlify Drop (mais fácil, sem conta)
1. Acesse **app.netlify.com/drop**
2. Arraste a pasta `orcamento-app` inteira para a página.
3. Pronto: ele gera um endereço tipo `seu-nome.netlify.app`. Guarde o link.

### Opção B — Vercel
1. Crie conta grátis em **vercel.com**.
2. *Add New → Project* e envie a pasta `orcamento-app` (ou conecte um repositório).
3. Recebe um endereço `.vercel.app`.

### Opção C — GitHub Pages
1. Crie um repositório em **github.com** e suba os arquivos da pasta.
2. *Settings → Pages → Branch: main → /root → Save*.
3. Fica em `seu-usuario.github.io/nome-do-repo`.

## 4. Sincronizar entre aparelhos
Como os dados ficam em cada navegador, para levar de um aparelho a outro:
- Na aba **Config → Exportar backup**, salve o arquivo `.json`.
- No outro aparelho, **Config → Importar backup** e selecione o arquivo.

Faça isso de vez em quando também como cópia de segurança.

## 5. Virar o ano (2027, 2028…)
O app tem **seletor de anos** no topo (‹ 2026 ›). Para criar o próximo ano é só tocar na seta **›** (ou no ano → *Criar 2027*). Ao criar:
- Receitas e despesas fixas já vêm **repetidas** (valores de referência de dezembro do ano anterior).
- Os **cartões começam zerados** para você lançar as faturas reais.
- O **saldo inicial** já vem preenchido com o **saldo final projetado do ano anterior**.

Cada ano fica salvo separado — você alterna entre eles quando quiser, sem perder nada. Se corrigir algo no ano anterior, use **Config → Puxar saldo do ano anterior** para reatualizar o saldo inicial.

---
**Privacidade:** nada é enviado para lugar nenhum — os números ficam só no seu navegador (e no backup que você baixar).
