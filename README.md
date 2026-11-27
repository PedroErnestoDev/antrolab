# AntroLab

Portal estático de ferramentas online gratuitas, desenvolvido com HTML5, CSS3 e JavaScript Vanilla.

## Desenvolvimento

Não há etapa de build. O projeto é servido diretamente pelo GitHub Pages.

## Publicação no GitHub Pages

1. Abra **Settings → Pages** no repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch principal e a pasta **/(root)**.
4. Salve e aguarde a publicação.
5. Em **Custom domain**, informe `antrolab.com.br` e confirme.
6. Configure no DNS do domínio os registros A para os endereços oficiais atuais do GitHub Pages e um CNAME de `www` para `PedroErnestoDev.github.io`.
7. Após a validação DNS, habilite **Enforce HTTPS**.

O arquivo `CNAME` já contém `antrolab.com.br`. Consulte a documentação oficial do GitHub Pages para os endereços IP atuais e instruções de DNS: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site

## Ferramentas implementadas

- Compressor de imagem: Canvas API, qualidade configurável e exportação.
- Conversor de imagem: exportação para WebP.
- Redimensionador: alteração de dimensões via Canvas.
- PNG para WebP e JPG para PNG.
- QR Code: biblioteca QRCode.js carregada via CDN.
- Contador de palavras e caracteres.
- Formatação de texto: caixa, capitalização e espaços.

## Observações importantes

- O utilitário PDF está identificado como indisponível; não anuncia operações ainda não implementadas.
- Os componentes publicitários estão reservados para integração futura. Nenhum código de anúncio foi inserido.
- Antes de lançar, revisar juridicamente as páginas de termos, privacidade e cookies, preencher os canais reais de contato e testar as ferramentas nos navegadores/dispositivos alvo.
- Bibliotecas externas são carregadas por CDN; para operação independente de terceiros, fixe versões e hospede os arquivos localmente após revisar suas licenças.
- Os caminhos absolutos iniciados por `/` pressupõem publicação na raiz do domínio personalizado antrolab.com.br.
