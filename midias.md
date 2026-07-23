Mídia em HTML5

Imagens e suporte visual

<img>: É uma tag vazia(void element) pois não possui tag de fechamento e não envolve texto ou conteúdo. Serve para inserir imagens na página e todo o seu comportamento é definido por seus atributos.
Os atributos essenciais são:
-src(source): Caminho relativo ou absoluto que leva a imagem.
-alt(alternative text): Descrição da imagem.
-width e height: Definem a largura e a altura da imagem em pixels.
- loading: Usado para adiar o carregamento da imagem somente quando o usuário estiver rolando para a posição da página onde a imagem se encontra.
    Ex: loading="lazy"
-title: Exibe uma legenda ou título quando o mouse passa por cima.
-deconding: Define se a imagem deve ser decodificada(renderizada) de forma:
    async: Assíncrona, ou seja o navegador vai baixar e decodificar a imagem em segundo plano, o restante da estrutura do site vai ser apresentada mesmo que a imagem ainda não tenha sido carregada.
    sync: Síncrona, ou seja o navegador irá carregar a imagem junto com o restante da página que será exibida somente quando a imagem tiver sido carregada.
    auto: Automática, permite que o navegador tome essa decisão.

Áudio e vídeos nativos

<audio>: É uma tag usada para reproduzir arquivos de som. É um elemento container(tag pai)
    <source>: Aninhada com a tag audio, serve para definir múltiplas alternativas de formato para o arquivo, o navegador irá carregar o primeiro compatível na lista. Permite a definição de um fallback que será retornado se nenhum dos formatos for compatível.
<video>: Tem a mesma sintaxe e comportamento da tag audio, adicionando alguns atributos específicos para vídeos.
Atributos de áudio e vídeo:
    -controls: Apresenta os controladores padrão do navegador, como play/pause, barra de carregamento e volume.
    -autoplay: Inicia a mídia automaticamente quando a página carrega.
    -muted: Inicia o áudio/vídeo no mudo.
    -loop: Reinicia a mídia quando chega ao fim.
    -preload: Define como o navegador deve carregar a mídia, se "none" não baixa até o usuário clicar no play. Se "metadata" carrega apenas as informações da mídia. Se "auto" baixa o arquivo inteiro imediatamente.
    -poster: Defime imagem de capa para o vídeo.
    -playsinline: Força o carregamento da mídia na estrutura da página e não em tela cheia.
    -track: Usada para legendas e acessibilidade com os seguintes atributos:
        -src: Caminho do arquivo de legenda ou acessibilidade.
        -kind: Define o tipo de faixa, podendo ser 'subtitle' para legenda, 'captions' para transcrição e efeitos especiais sonoros, ou 'descriptions' para audiodescrição.
        -srclang: Código de idioma.
        -label: Nome do idioma que será exibido entre as opções.
        -defalt: Define qual legenda virá ativada por padrão.

Incorporação externa e objetos

<iframe>: Janela para incorporar documentos html ou página web completas.
Os atributos essenciais são:
    -src: A url do recurso externo.
    -title: O título do documento html ou da página.
    -allow: Define que o iframe tenha permissões de acesso à recursos do dispositivo.
    -sandbox: Define restrições de acesso do iframe a ações e recursos.
<embed>: Usada para integrar conteúdos e mídias externas.
<object>: Semelhante a embed porém permite especificar um fallback a ser exibido caso não seja possível carregar o conteúdo.