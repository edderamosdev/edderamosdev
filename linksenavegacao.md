Links e Navegação em HTML5

Fundamentos da tag de âncora

É um elemento inline que se torna clicável e faz conexões da página atual com outras páginas ou recursos.

A estrutura básica é:
<a href="destino">Texto ou conteúdo clicável</a>
Onde:
a=Âncora, elemento pai
href=Hypertext reference, o destino

O destino pode ser um endereço absoluto ou relativo. O destino absoluto é usado para links externos e deve ser informado na sua forma completa incluindo o protocolo https://www...

O destino relativo é usado para navegação interna dentro do mesmo projeto. Não precisa do protocolo mas apenas do arquivo ou caminho das pastas do repositório local.

O atributo target define onde o link será aberto, abrindo uma novs guia ou aba no navegador.

target="_blank"

Para maior segurança usamos o atributo rel para cortar a interção entre a nova página e a página oringinal.

rel="noopener noferrer"

Podemos criar âncoras para a mesma página afim de levar o usuário a posições diferentes do conteúdo. Para isso basta atribuir um id ao elemento e referenciar o id dentro da âncora iniciando com o #.

O # também pode ser utilizado sozinho para levar o usuário de volta ao topo da página.

Prefixos especiais:

- mailto: Redireciona o usuário ao aplicativo de email padrão.
Sintaxe básica:
<a href="mailto:contato@exemplo.com">Envie um email</a>

Além da sintaxe básica podemos inserir parâmetros pra pré-preencher os campos do email.

?subject=Define o assunto do email

&body=Define o texto do corpo do email

- tel: Redireciana o usuário para o aplicativo de discagem
Sintaxe básica:
<a href="tel:+5585999258184">Ligue pra mim</a>

- download: Muda o comportamento do navegador que ao invés de abrir o link irá baixar o arquivo.
Sintaxe básica:
<a href="manuais/guia-do-usuario.pdf" download>Baixar</a>

O atributo download pode receber um valor que irá sugerir um nome para o arquivo. Para isso basta adicionar="Nome-do-arquivo" depois do atributo download.