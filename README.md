# Universo Elétrico — Mídias Públicas

Este repositório contém **somente as imagens destinadas a distribuição pública** do perfil Universo Elétrico. Ele não contém código do robô, chaves de API, histórico de usuários ou dados privados.

## Publicar imagens

No GitHub, acesse **Settings → Pages → Build and deployment**, escolha **Deploy from a branch**, depois **main** e **/docs**, e clique em **Save**.

Depois que o GitHub Pages ficar ativo:
- Post: `https://universoeletrico.github.io/Universo-Eletrico-Midia/posts/001.jpg`
- Carrossel: `https://universoeletrico.github.io/Universo-Eletrico-Midia/carousels/CR001/01.jpg`

Esses são **endereços esperados** e devem ser testados antes de atualizar os links do robô.

## Sincronização futura

O projeto principal possui um workflow preparado em `.github/workflows/sincronizar-midias.yml` para copiar apenas os arquivos de `docs/posts`, `docs/carousels` e alguns arquivos visuais públicos, sem apagar imagens já publicadas. Para funcionar depois que o código principal ficar privado, precisa de um secret `MEDIA_REPO_TOKEN` no repositório principal, com permissão **Contents: Read and write** apenas para **Universo-Eletrico-Midia**.

**Nunca coloque tokens em arquivos deste repositório público.**
