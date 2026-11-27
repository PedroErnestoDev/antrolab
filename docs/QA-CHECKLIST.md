# AntroLab — checklist de qualidade

Este checklist separa revisão estática de testes reais no navegador. Os itens abaixo não devem ser considerados aprovados até serem executados em ambiente publicado ou local.

## Interface e navegação
- [ ] Página inicial em 360 px, 390 px, 768 px, 1024 px e desktop.
- [ ] Menu mobile abre e fecha; links navegam corretamente.
- [ ] Alternância claro/escuro persiste após atualizar a página.
- [ ] Catálogo: busca por nome, descrição e tags.
- [ ] Catálogo: filtros Todas, Imagens, Texto e Utilidades.
- [ ] Todos os cartões levam a uma página existente.
- [ ] Cabeçalho, rodapé, consentimento de cookies e anúncios não se sobrepõem.

## Ferramentas de imagem
Executar em JPG, PNG com transparência e WebP:
- [ ] Compressor: seleção por botão e arrastar/soltar.
- [ ] Compressor: qualidade configurável em JPEG/WebP; PNG é exportado como WebP para permitir compressão ajustável.
- [ ] Conversor: selecionar PNG, JPEG e WebP; validar MIME e extensão reais do arquivo baixado.
- [ ] PNG para WebP: aceitar PNG e rejeitar JPG/WebP; arquivo baixado abre e mantém dimensões.
- [ ] JPG para PNG: aceitar JPG/JPEG e rejeitar PNG/WebP; arquivo baixado abre e fundo é tratado corretamente.
- [ ] Redimensionador: dimensões personalizadas, proporção ligada/desligada e limites.
- [ ] Prévia, metadados, mensagens de erro e download funcionam.
- [ ] Testar arquivo inválido, arquivo acima de 30 MB e imagem acima de 40 MP.
- [ ] Testar navegadores Chromium, Firefox e Safari/WebKit, desktop e Android.

## PDF
- [ ] A página PDF permanece identificada como indisponível e não aparece no catálogo até existir implementação real.

## Texto e QR Code
- [ ] Contador com texto vazio, acentos, emojis, quebras de linha e pontuação.
- [ ] Formatador: cada transformação, preservação de acentos e cópia.
- [ ] QR Code: URL, texto simples, tamanhos disponíveis e download PNG.
- [ ] Comportamento quando a biblioteca CDN não carrega.

## SEO, privacidade e monetização
- [ ] Títulos, descrições, canonical, sitemap.xml e robots.txt.
- [ ] Política de privacidade, cookies e termos revisados juridicamente.
- [ ] Consentimento: rejeitar, aceitar apenas anúncios, aceitar tudo e reabrir preferências.
- [ ] Google Analytics só carrega após consentimento correspondente.
- [ ] Anúncios só carregam conforme o consentimento e as configurações aprovadas.
- [ ] Validar no Adsterra as categorias bloqueadas e testar a entrega real dos anúncios.

## Critérios para publicação
- Nenhum link quebrado ou ferramenta anunciada sem implementação.
- Nenhum erro JavaScript no console durante os fluxos principais.
- Arquivos baixados devem abrir e corresponder ao formato anunciado.
- Testes de layout devem ser feitos em dispositivos reais.
- Não afirmar que a suíte está aprovada sem executar os itens acima.
