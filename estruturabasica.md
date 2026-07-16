A respeito da estrutura básica de um arquivo HTML

Todo arquivo HTML deve ser inicializado com a declaração <!DOCTYPE html>, Document Type Declaration(declaração do tipo de documento). Essa tag define a página como sendo do formato HTML 5. É a primeira linha de código justamente para que o navegador inicie a execução seguindo os padrões mais modernos da linguagem.

É importante não confundir a declaração doctype com a tag <html> que continua sendo utilizada obrigatóriamente no início e no fim de toda página HTML. A tag <html> pode ser utilizada com alguns atributos, sendo os mais comuns:

<html lang="pt-BR">
O atributo 'lang' é a abreviação de language, e define o idioma principal da página. É de uso obrigatório nas boas práticas pois esse atributo será interpretado pelo navegador, pelos motores de busca e pelas ferramentas de acessibilidade.

Além do atributo lang, outro atributo muito utilizado para a tag <html> é o atributo dir.
<html dir="ltr">
Esse atributo define a direção do texto podendo ser left to right(ltr) ou right to left(rtl). Geralmente é utilizado quando o idioma principal da página é árabe ou asiático, que são lidos detrás para frente.

A tag <html> ainda pode ser utilizada com atributos globais como class ou id, caso haja a necessidade de definir características diferentes a serem herdadas em cascata por todos os elementos da página, considerando que a tag html envolve todos os elementos.

Um exeplo interessante é o dark mode, ou tema escuro, sendo possível definir uma classe na tag html que irá conter os mesmo elementos contudo com as características definidas para o tema escuro. Será utilizado um pequeno script Javascript para adicionar ou remover esse atributo quando usuário seleciona a opção claro ou escuro.

Outra aplicação útil é o atributo id, que pode ser utilizado quando uma página específica precisa de uma modificação exclusiva na estrutura ou elementos. Para evitar de ter que desenvolver outra página, podemos apenas definir um atributo id e aplicar as mudanças na página desejada mantendo todo o resto da estrutura e da folha de estilo.

---

A tag <head>, em inglês 'cabeça', é a tag destinada aos metadados, ou seja as configurações técnicas da página que são interpretadas pelo navegador e pelos motores de busca, mesmo que essas informações não seja exibidas ao usuário.

Entre os metadados mais comuns estão:

<meta charset="UTF-8">
Define como o navegador vai decodificar o texto com acentos e cedilha.

<meta name="viewport" content="width=device-width, initial-scale=1.0">
Permite a responsividade com a largura dinâmica da página que será capaz de se adaptar para dispositivos móveis.

<title>Meu título</title>
Define o título da página.

<meta name="description" content="Breve descrição do site ou da página">
Permite adicionar uma descrição da página que poderá ser exibida em pesquisas ou ser lido por uma ferramenta de acessibilidade.

Seguindo essa mesma sintaxe, mudando apenas o valor 'name', também temos os metados:
keywords: palavras-chave
author: autor da página ou do conteúdo
robots: Definie se os motores de buscam devem indexar(index: armazenar o conteúdo da página e exibir nas pesquisas) e se deve seguir(follow: abrir os links presentes na página e explorar o conteúdo que há neles)
favicon: Não é um metadado mas sim um atributo da tag <link> e serve para definir o ícone de uma página. A sintaxe é <link rel="icon" href="imagem.png" type="image/png">