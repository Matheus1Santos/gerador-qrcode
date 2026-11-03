# Link em QR

Gerador de QR codes em uma página HTML, em português, responsivo e sem servidor.

## Usar

Baixe `index.html` e abra no navegador. Cole um link, clique em **Gerar QR code** e baixe a imagem em **PNG** ou **SVG**. A biblioteca está incluída no HTML: não é necessário instalar dependências nem ter internet para gerar os códigos. O destino do link pode exigir internet para ser acessado.

Os links são processados localmente, sem serviços de QR code, cadastro ou rastreamento. O QR code contém diretamente o endereço e não tem expiração própria; o endereço de destino precisa continuar disponível.

## Publicar com GitHub Pages

1. No repositório, abra **Settings → Pages**.
2. Em **Build and deployment**, escolha **Deploy from a branch**.
3. Selecione **main** e **/ (root)** e clique em **Save**.
4. Aguarde o GitHub mostrar o endereço publicado.

Endereço esperado depois da ativação: https://matheus1santos.github.io/gerador-qrcode/

## Verificação

Testes automatizados decodificaram os QR codes de quatro URLs, incluindo parâmetros, acentos e domínio internacional. Também verificaram as ações de download PNG/SVG, a invalidação do resultado ao editar o link e seis casos de entrada inválida. A aparência ainda não foi verificada em navegador real.

## Biblioteca

Inclui [qrcode-generator 2.0.4](https://github.com/kazuhikoarase/qrcode-generator), de Kazuhiko Arase, sob licença MIT. Consulte `THIRD-PARTY-LICENSE.txt`.
