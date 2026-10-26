# ENTREGA — Atividade 4 (PWA)

> Preencha e faça commit junto com o código. Esta parte vale 3 pts (avaliação manual no Canvas).

**Nome:** Gabriel Campos Ferreira Lisboa · **GitHub:** gabrielcflisboa

---

## 1. Site comum × PWA — o que EU vi (3 diferenças)

Abra `https://pwa-tmdb-aula4.vercel.app` e compare com um site comum (ex.: themoviedb.org). Modo avião → recarregar; fechar e reabrir; instalar.

| # | Site comum | PWA | Print/evidência |
|---|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

## 2. Prova do offline no SEU build

- [ ] Print do **DevTools → Application → Cache Storage** com `tmdb-api` e `tmdb-images` (com itens)
- [ ] Print do app em **modo avião** carregando a lista
- [ ] Print do aviso **"Nova versão disponível"** (ou explique por que não conseguiu reproduzir)

(Coloque os prints numa pasta `evidencias/` e referencie aqui.)

## 3. Reflexão (5–8 linhas)

`autoUpdate` × `prompt`: qual você escolheria para um app de **checkout** e para um app de **notícias**, e por quê? O que pode dar errado em cada escolha?

Para um app de **checkout** eu escolheria `prompt`: com `autoUpdate` o app pode recarregar no meio de um pagamento e o usuário perder o carrinho ou o formulário, ou ficar com JS novo conversando com uma API antiga. Com `prompt` o usuário atualiza quando termina a compra; o risco é ele nunca aceitar e ficar preso numa versão velha (com bug ou falha de segurança), então convém forçar a atualização em versões críticas.

Para um app de **notícias** eu escolheria `autoUpdate`: não há estado sensível a perder, o conteúdo é só leitura e é melhor que todos vejam sempre a versão mais recente sem fricção. O risco é a página recarregar sozinha enquanto a pessoa lê um artigo, ou uma versão com bug ir para todos de uma vez.

## 4. Declaração de uso de IA

Usei IA? Onde e como? (uso transparente é incentivado)

Usei o GitHub Copilot (assistente de IA) para implementar os TODOs 1–5 e redigir a reflexão; rodei `npm test` e `npm run build` para validar. Os prints de evidência (seções 1 e 2) precisam ser feitos manualmente no navegador.
