# FÉ FLIX — aplicativo Android

Primeira versão de um feed vertical de vídeos cristãos descobertos automaticamente no YouTube.

## Recursos
- Feed vertical com vídeos incorporados do YouTube.
- Pesquisa por categorias: Jesus, pregações, louvores, estudos bíblicos, testemunhos e profecias.
- Pesquisa livre no YouTube.
- Salvar vídeos localmente e compartilhar links.
- Interface adaptada para celular.

## Requisito para a busca automática
A busca usa a YouTube Data API v3. É necessário criar uma chave no Google Cloud Console:
1. Crie um projeto em https://console.cloud.google.com/
2. Ative **YouTube Data API v3**.
3. Crie uma credencial do tipo **API key**.
4. Abra o app, toque na engrenagem e cole a chave.

A chave é armazenada no armazenamento local do aplicativo. Restrinja a chave à YouTube Data API v3 e configure limites de cota no Google Cloud. A API tem cota diária; buscas frequentes podem consumir essa cota.

## Gerar APK pelo GitHub usando o celular
1. Crie um repositório no GitHub e envie todos os arquivos desta pasta.
2. Abra a aba **Actions** do repositório.
3. Selecione **Gerar APK Android** e toque em **Run workflow** (ou faça push na branch `main`).
4. Quando terminar, abra a execução e baixe o artefato **fe-flix-apk**.
5. Extraia o APK e instale no Android.

## Observações
- Os vídeos são encontrados e reproduzidos pelo YouTube; o app não baixa nem hospeda vídeos.
- O YouTube controla disponibilidade, anúncios, direitos autorais e restrições de incorporação.
- A pesquisa automática não garante que todo resultado seja doutrinariamente correto ou exclusivamente cristão. Esta versão usa termos cristãos, `safeSearch=strict` e vídeos incorporáveis; recomenda-se evoluir para curadoria/moderação.
- Esta é uma versão inicial. Curtidas, comentários, contas e sincronização entre aparelhos ainda não estão implementados.
