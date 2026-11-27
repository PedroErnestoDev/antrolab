# AntroLab

Portal de ferramentas online gratuitas, desenvolvido com HTML5 semântico, CSS3 e JavaScript Vanilla (ES6+). O projeto é estático e publicado pelo GitHub Pages, sem etapa de build.

## Experiência e arquitetura

- Interface responsiva com tema claro/escuro.
- Catálogo pesquisável e filtros por categoria.
- Navegação e componentes compartilhados gerados por JavaScript.
- Ferramentas executadas no navegador sempre que possível.
- Preferências de tema, histórico e consentimento armazenados localmente.
- Integrações de Google Analytics 4 e Adsterra carregadas conforme as preferências de consentimento.

## Ferramentas

- Compressor de imagens JPG, PNG e WebP, preservando o formato original.
- Conversor de imagens entre PNG, JPEG e WebP.
- Redimensionador de imagens com controle de proporção.
- Conversão PNG para WebP e JPG/JPEG para PNG.
- Gerador de QR Code.
- Contador de palavras, caracteres, frases e parágrafos.
- Formatador de texto.

O recurso de PDF permanece fora do catálogo enquanto não houver implementação funcional.

## Publicação no GitHub Pages

1. Em **Settings → Pages**, selecione **Deploy from a branch**.
2. Escolha a branch principal e a pasta **/(root)**.
3. Confirme o domínio personalizado `antrolab.com.br`.
4. Configure os registros DNS conforme a documentação oficial do GitHub Pages.
5. Após a validação, habilite **Enforce HTTPS**.

O arquivo `CNAME` contém `antrolab.com.br`. Consulte: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site

## Qualidade e manutenção

- O workflow em `.github/workflows/quality.yml` executa verificações de sintaxe JavaScript.
- A lista de testes manuais está em `docs/QA-CHECKLIST.md`.
- Antes de publicar mudanças, testar as ferramentas em navegadores desktop e mobile.
- Revisar periodicamente políticas de privacidade, cookies e termos. O canal de contato deve refletir um endereço real e monitorado.
- Bibliotecas externas são carregadas por CDN; fixe versões e avalie hospedagem local se for necessário reduzir dependências de terceiros.

Os caminhos absolutos iniciados por `/` pressupõem publicação na raiz do domínio personalizado `antrolab.com.br`.
