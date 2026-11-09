# Renda Fixa da Semana – Vulture Capital

Página pública (celular primeiro) com indicadores, sugestão de alocação por perfil, aplicações da semana, comentário e resumo do mercado. Tudo vem do arquivo `dados.json`.

| Arquivo | Para quê |
|---|---|
| `index.html` | Página que o cliente abre pelo link do WhatsApp |
| `admin.html` | Tela de administração: edita aplicações, alocação, indicadores e textos e publica no GitHub |
| `dados.json` | Conteúdo da página |
| `assets/` | Ícone e imagem de pré-visualização do link no WhatsApp |

## Colocar no ar (uma vez)
1. Repositório público `vulturecapital/vulturecapital.github.io` com estes arquivos na raiz.
2. **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.**
3. Endereço: **https://vulturecapital.github.io/** (administração: https://vulturecapital.github.io/admin.html).

## Token para a tela de administração (uma vez)
GitHub → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**
- Repository access: *Only select repositories* → este repositório
- Permissions → Repository permissions → **Contents: Read and write**
- Copie o token e cole em `admin.html` (fica salvo só no seu navegador).

## Rotina semanal
- **Aplicações e alocação (você):** abra `…/admin.html`, ajuste ou cole o bloco de produtos da planilha (B3:B29) em *Importar da planilha* e clique em **Publicar no site**. A página atualiza em cerca de 1 minuto.
- **Resumo do mercado, comentário, indicadores e Focus (Claude):** atualizados no `dados.json` a cada semana, junto com a aba *Resumo do Mercado* da planilha.

Se as duas edições acontecerem ao mesmo tempo, a tela de administração avisa antes de sobrescrever.
