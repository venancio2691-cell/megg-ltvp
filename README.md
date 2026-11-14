# MEGG LTVP

App de inspeção predial / autovistoria (Rio de Janeiro) para engenheiros: checklist por sistema, constatações com fotos, classificação (NBR 16747, GUT, IBAPE), laudo em PDF/DOCX e assistente de IA.

## Como funciona
- `index.html` é o app inteiro (web e Android usam o mesmo arquivo).
- A cada `push` na branch `main`, o GitHub Actions:
  1. publica o site no GitHub Pages (`https://SEUUSUARIO.github.io/vistoria-ltvp/`);
  2. gera o APK Android com Capacitor e publica na release **latest** (`.../releases/latest/download/MEGG_LTVP.apk`).

## Ativar (uma vez)
1. Settings → Pages → Source: **GitHub Actions**.
2. Settings → Actions → General → Workflow permissions: **Read and write**.
3. Actions → "Build web + APK" → Run workflow.

## IA
No site/APK, toque em ✨ IA e informe uma chave da API da Anthropic (console.anthropic.com). Dentro do claude.ai não precisa de chave.
