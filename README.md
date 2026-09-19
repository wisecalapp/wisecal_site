# WiseCal

Site institucional estático em português, adaptado do arquivo `Website WiseCal.zip`. Preserva o conteúdo, as cores, o fundo e os cartões do layout fornecido, com ajustes para celular e acessibilidade.

## Visualizar

Abra `index.html` no navegador. Não é necessário instalar Node.js, executar um build ou configurar servidor. O conteúdo e os ícones funcionam sem JavaScript. A fonte Plus Jakarta Sans vem do Google Fonts; se estiver indisponível, o site usa uma fonte do sistema.

## Publicar no GitHub Pages pelo navegador

1. Entre no GitHub e crie um repositório **público**, por exemplo `wisecal`.
2. No repositório, use **Add file → Upload files**.
3. Envie `index.html`, `styles.css`, a pasta `assets`, `.nojekyll` e este `README.md`. Envie os arquivos extraídos, não o ZIP. O `index.html` deve ficar diretamente na raiz do repositório, não dentro de outra pasta. Se o navegador não enviar `.nojekyll`, use **Add file → Create new file** para criá-lo; pode conter apenas uma linha em branco.
4. Clique em **Commit changes** para salvar na branch `main`.
5. Abra **Settings → Pages**.
6. Em **Build and deployment → Source**, selecione **Deploy from a branch**.
7. Em **Branch**, selecione **main** e **/(root)**. Clique em **Save**.
8. Aguarde a publicação. A página **Settings → Pages** mostrará o link. Para o exemplo acima, o endereço será `https://SEU-USUARIO.github.io/wisecal/`.

Para atualizar o site, envie novamente os arquivos alterados e salve o commit. O GitHub Pages publica as mudanças automaticamente. Se houver erro, confira a execução na aba **Actions** e verifique se `index.html` está na raiz e se a branch configurada está correta.

Os caminhos de CSS e favicon são relativos, portanto funcionam também em repositórios com outros nomes ou em um domínio próprio.

Referência oficial: [Configurar a origem de publicação do GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Personalizar

- **Textos e conteúdo:** `index.html`.
- **Cores, espaçamentos e adaptação para celular:** `styles.css`.
- **Ícone da aba:** `assets/favicon.svg`.
- **Downloads:** os dois botões estão desabilitados, como no material original. Quando tiver os endereços oficiais, substitua cada `<button ... disabled>...</button>` por `<a class="store-button" href="URL-OFICIAL">...</a>`, remova os avisos de lançamento e acrescente `text-decoration: none` à classe `.store-button` no CSS.
- **Rodapé:** atualize o ano em `index.html` quando necessário.

O cartão de calorias é uma prévia ilustrativa. Este projeto é o site de apresentação; não implementa o aplicativo, identificação de refeições ou armazenamento de dados.

## Arquivos de referência

A pasta local `source-reference` contém a extração do ZIP original para consulta. Ela está ignorada pelo Git e não é necessária para publicar. Os componentes proprietários do editor foram substituídos por HTML, CSS e SVG nativos. Nenhum código do editor é executado pelo site final.
