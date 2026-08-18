<p align="center">
  <img src="assets/header.svg" alt="Caio Demartine" width="100%">
</p>

<p align="center">
  <a href="https://argosleads.com"><img alt="argosleads.com" src="https://img.shields.io/badge/argosleads.com-C6A15B?style=flat-square&labelColor=101820&color=C6A15B"></a>
  <a href="https://github.com/caiobelatodemartine-cmd/argos"><img alt="Argos" src="https://img.shields.io/badge/vitrine%20do%20Argos-101820?style=flat-square&labelColor=101820&color=4F5D4E"></a>
</p>

<br>

Construo software que precisa sobreviver fora da minha máquina: instalador que
roda no Windows de outra pessoa, banco que isola um cliente do outro, licença que
não dá para burlar com o inspetor do navegador, texto legal que aguenta a LGPD.

A maior parte do meu trabalho é privada. O que dá para mostrar está abaixo.

<br>

## No que estou trabalhando

<table>
<tr>
<td width="120" valign="top">
  <img src="assets/argos-mark.svg" alt="" width="88">
</td>
<td valign="top">

### [Argos](https://github.com/caiobelatodemartine-cmd/argos)

**Prospecção B2B local para Windows.** Encontra empresas reais por nicho e cidade,
cruza com o cadastro de CNPJ da Receita Federal, pontua o encaixe com IA e monta
listas prontas para contato.

Electron e React na frente, SQLite cifrado na máquina do cliente, Supabase apenas
para conta e direito de uso. O envio nunca é automático: a busca para em `review` e
o disparo exige confirmação manual, porque outreach automático queima o domínio de
quem comprou.

<sub>Electron · React · TypeScript · SQLite · Supabase · Stripe · Gmail API · 691 testes</sub>

</td>
</tr>
</table>

<br>

## Stack

| Camada | O que eu uso |
| --- | --- |
| **Desktop** | Electron, React, Vite, TypeScript, Tailwind |
| **Backend** | Postgres com RLS, Edge Functions em Deno, Supabase Auth |
| **Dados** | SQLite com better-sqlite3, Drizzle, AES-256-GCM para PII |
| **Integrações** | Stripe, Gmail API, OpenStreetMap, Apify, Claude, GPT, Gemini |
| **Web** | HTML e CSS escritos à mão, CSP estrita, Apache |
| **Teste** | Vitest, Playwright, red team multiagente |

<br>

## Como eu trabalho

**Lógica pura no contrato, efeito colateral na borda.** Quota, licença e template
não tocam disco nem rede, então rodam em teste sem subir a aplicação. É o que
permite uma suíte de centenas de testes que roda em segundos.

**O comentário explica a decisão, não o código.** Se está escrito no arquivo, é
porque alguém no futuro ia desfazer aquilo sem saber o que quebra.

**Segurança é fronteira, não camada.** O que o servidor não guarda não vaza. O que
é verificado por assinatura não se falsifica apontando o domínio para `localhost`.

**Nenhum segredo entra no Git.** Nem uma vez, nem em branch de teste. O histórico
guarda para sempre.

<br>

---

<p align="center">
  <sub>
    Fale comigo por <a href="https://argosleads.com">argosleads.com</a>.
  </sub>
</p>
