Sobre formatação de texto em HTML

A formatação de texto em HTML é feita envolvendo o conteúdo em tags de formatação. Essa formatação não é apenas visual mas também tem a função de atribuir significado, hierarquia e semântica ao conteúdo.

Todos os elementos visíveis da página devem ficar envolvidos pela tag <body> que nada mais é que "corpo" em inglês. Aqui estará contido todas as tags da linguagem mas sendo um contesúdo extenso começaremos por partes primeiramente com a formatação de texto.

- Ênfase e importância
<strong>: Negrito e significado semântico de maior importância se comparado ao resto do texto.

<em>: Emphasis, itálico e significado semântico de enfânse que pode ser interpretado por leitores de acessibilidade.

<b>: Bold, apenas negrito sem significado semântico

<i>: Italic, apenas itálico sem significado semântico

- Modificações e correções

<ins>: Inserted, texto sublinhado com significado semântico que indica que foi inserido posteriormente.

<del>: Delete, texto tachado ou riscado com significado semântico que indica que foi removido.

<sub> e <sup>: Texto subescrito e supraescrito.

- Estrutura e hierarquia

<p>: Parágrafos, bloco fundamental para textos

<br>: Breakroll, quebra de linha

<h1> ao <h6>: Títulos hierárquicos que denotam a ordem de importância do conteúdo e também alteram o tamanho do texto.

<hr>: Horizotal roll, linha horizontal de separação de conteúdo.

- Citações e referências

<blockquote>: Citação longa e separada do restante do texto, por ser um elemento do tipo block-level.

<q>: Citação curta que é apresentada dentro da mesma linha, por ser um elemento inline.

<cite>: Citation title, citação de título de obra.

<abbr>: Abbreviation, abreviação

- Formatações técnicas

<code>: Bloco de código

<pre>: Bloco de código pré-formatado

<kbd>:Keyboard, indica texto de interação do usuário(entrada de teclado)

- Internacionalização e direção de texto

<bdo>: Bi-directional override, determina a direção do texto e deve ser usado obrigatóriamente com o atributo dir, sendo rtl(right to lefth) ou ltr(lefht to right).

<bdi>: Bi-directional isolation, isola o texto de formatação especial desconhecida afim de que não seja alterado pelos atributos gerais da página.

<ruby>, <rt> e <rp>: Ruby é uma formatação destinada a ocasiões onde é necessário apresentar a pronúncia ou anotação junto a uma palavra principal. Sendo <ruby> a tag mãe que contém o texto principal, e <rt> a tag que contém a anotação. Como alternativa para navegadores antigos pode-se utilizar também o <rp> para exibir os parênteses com a anotação ao lado, mas navegadores modernos ignoram o <rp>.