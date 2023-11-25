# Anotações importantes / Desafio de Projeto DIO

Repositório para armazenar e compartilhar informações que estou aprendendo ao longo do projeto Potência Tech iFood - Desenvolvimento de Jogos, da  [Digital Inovation One](https://www.dio.me/).
# Git & GitHub
## 🧑‍💻 Comandos Importantes Git
```
 git init - Inicia o git no repositorio
 git clone <URL> - Copia repositorio remoto
 git status - Lista as modificações atuais do repositório 
 git log - Lista histórico de commits
 git add <nome-arquivo> - Adiciona o arquivo do palco(stage)
 git reset <nome-arquivo> - Remove o arquivo do palco(stage)
 git commit m"mensagem" - Realiza o commit das modificações
 git branch - Lista todas as branch locais 
 git branch <nome-da-branch> - Cria uma nova branch 
 git checkout <nome-da-branch> - Entra na branch
 git pull original <nome-da-branch> - Pucha as modificações
 git push origin <nome-da-branch> - Envia as modificações para o repositorio remoto

```


## 💾 Downloads
- [Download GIT](https://git-scm.com/downloads)
- [Download GITHUB](https://desktop.github.com/)


## 📖 Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/)

# HTML

# CSS
- link rel="stylesheet" href="/aaa/css/style.css (por exemplo), essa tag que é usada para importar nosso css de uma folha externa.
- object-fit (propriedade para imagens). object-fit: fill;(padrão) ele estica ou diminui a imagem para fazer ela caber no container, porém geralmente a imagem fica distorcida. object-fit: contain; a imagem vai ser redimensionada para caber no container, sem distorcer(sem perder qualidade) porém pode nao ocupar todo o espaço do container. object-fit: cover; a imagem vai preencher todo o container, porém ao invés de ficar distorcida ela vai cortar o espaço da imagem que ultrapassar o espaço que o elemento tem, assim mantendo a qualidade da imagem, porém dependendo da imagem pode-se perder uma parte da imagem devido ao corte. object-fit: none; a imagem vai ignorar a altura e largura do elemento pai, assim tendo sua proporção de origem. object-fit: scale-down; ele vai escolher entre o countain e o none, qual das duas configurações vai ser a menor assim a aplicando. Altera a posição da img object-position: x y; podem ser %, pixels(px), left, top, center, right, bottom, etc.
- background-image: url('...'); serve para utilizar uma imagem como background (todos os formatos de imagem sao aceitos ate gifs).
- linear-gradient(purple, red) esse efeito aplica uma troca de cor no elemento, um efeito linear, idealmente usada do mesmo tom por exemplo um rosa claro e um rosa mais escuro (podem conter mais de duas cores).
- radial-gradient(purple, red) proximo do efeito linear porem em circulo.
- repeat-linear-gradient ou repeat-radial-gradient sao outras funçoes de fundo cor, listras.
- dica: da para colocar uma imagem sobre a outra.
- background-size: que pode ter como atributos : auto(automatico) vai se ajustar automaticamente ao elemento, porem se a imagem for muito grande ela nao se adapta. cover(cobrir) ocupa todo o fundo do nosso elemento mesmo se a imagem for maior ou menor que o container, porém pode ser que ela corte um pouco da imagem original para caber dentro do container, tambem perde qualidade se a diferenca de tamanho for muito grande. contain redimenciona o tamanho da imagem para fazer ela aparecer inteira, cobre a parte que conseguir. pode ser utilizado com px e % também, com um unico valor exemplo 50% define a largura, a altura sera automatica, passando dois valores ocupara largura e altura, por exemplo 200px 250px, tomar cuidado para nao esticar muito a imagem, fazendo perder qualidade.
- background-repeat essa propriedade define se a imagem deve-se repetir, verticalmente, horizontalmente, ou nao repetir, veja os atributos dessa propriedade: background-repeat: repeat; (é o comportamento padrao, fazendo a imagem se repetir na horizontal e na vertical. background-repeat: repeat-x; repete apenas na horizontal. background-repeat: repeat-y; repete apenas no eixo vertical. background-repeat: space; com esse valor a imagem vai se repitir nas duas direções tanto vertical como horizontal sem cortar a imagem e com um espaço em branco entre elas evitando corte de imagem. background-repeat: round; repete em ambos os eixos e redimenciona para caber a imagem inteira sem cortar, porem geralmente perde qualidade. background-repeat: no-repeat; faz com que a imagem nao se repita em nenhum dos eixos. Da para aplicar tambem dois atributos um para o eixo x e outro para o eixo y, por exemplo: background-repeat: round space;.
- background-position essa propriedade serve para posicionar o background, imagem, etc.. exemplos: background-position: top; / bottom, left, right, center, top left, bottom right, também pode usar px e %. Com px e % da pra separar por horizontal e vertical com dois atributos exemplo: 10px 30px; 20px 80%; left 15px; bottom 10px right 20px; etc..
- background-attachment essa propriedade vai definir como o fundo do nosso elemento vai se movimentar em relação a janela do navegador e tem como valores: background-attachment: fixed; com esse atributo a imagem vai continuar fixa enquanto o texto se move por exemplo, faz um efeito legal. background-attachment: scroll; quando rolar a pagina ele da efeito como se a iamgem fosse embora junto com o scroll da pagina. background-attachment: local;  a imagem scrolla junto com os elementos, e fica fixa pro scroll da pagina.
- background-origin essa propriedade permite definir o ponto de origem de uma imagem de fundo. background-origin: padding-box; valor padrao da propriedade, ponto de origem no canto superior esquerdo do espaçamento interno que é o padding, com esse valor a imagem nao cobre a borda, mas cobre a area que o padding ocupa. background-origen: border-box; começa da esquerda canto superior e vai cobrir alem do espaçamento interno do nosso elemento e tambem a area que a borda se encontra. background-origin: content-box; começa esquerda lado superior porém ela nao vai cobrir a area da nossa borda nem do espaçamento inteno que é o padding, entao ela cobre apenas o espaço do conteúdo.
- background-clip essa propriedade é semelhante a propriedade origin, ela permite controlarmos nossa imagem se ela deve preencher as areas do espaçamento interno, a borda, ou o conteúdo tambem. background-clip: padding-box; nosso fundo nao vai preencher a area da borda do elemento, porem cobre a parte do padding. background-clip: border-box; com esse valor ele preenche toda a area, borda e padding. background-clip: content-box; preenche apenas o conteudo, nao preenche o padding nem a border. background-clip: text; esse efeito aplica o fundo de forma com que o background ocupe o espaço do texto e nao pro fundo da imagem, dando um background diretamente nas letras do conteudo, detalhe: deve-se aplicar a cor do testo como transparent, para o efeito funcionar, tambem indica-se usar assim: -webkit-background-clip: text; pra atingir mais navegadores.
- background-blend-mode essa propriedade permite mesclar nossos fundos, por exemplo coloco uma imagem de fundo background-imagem: url('...'); e background-color: orange; entao o atributo background-blend-mode-multiply; mescla os dois fazendo a imagem de fundo pegar a coloração orange. existem diversos atributos que podem ser colocados com essa propriedade, cabe aprofundar se necessário, alguns exemplos: multiply, overlay, screen, darken, lighten, color-dodge, color-burn, hard-light, soft-light, difference, exclusion, hue, saturation, color, luminosity.
- background: você pode definir diversas propriedades citadas acima somente usando o background, exemplo: background: (primeira camada) url('...') top-center / 200px 200px no-repeat fixed padding-box content-box red , (segunda camada) url('...') blue left repeat fixed padding-box;.
- border, assim como o background pode ser usado em uma unica linha ou separado as suas propriedades, que são: border-width: 10px; ou border-widht: 15px 20px 4px 30px; ou border-width: thin; ou border-width: medium; ou border-width: thick; por exemplo. < É a espessura da borda!.  temos o (define um estilo para a borda)border-style: solid; border-style:none;(e o padrão), border-style: dashed; border-style: dotted; border-style: double; border-style: groove; border-style: ridge; border-style: inset; border-style: outset;. é possivel aplicar bordas mistas, por exemplo: border-style: dotted dashed solid groove;. border-color: purple; também é possivel colocar cores mistas por exemplo: border-color: green, red, blue, black;. Usando as propriedades em uma unica linha seria: border: 10px solid green;(respectivamente width, style e color), Aplicando em apenas um lado da borda = border-bottom: , border-top:, border-right:, border-left:, border-bottom-widht: , etc..
- border-radius é a propriedade que arredando os cantos da borda, quanto maior o numero mais arredondado vai ser, exemplo = border-radius: 20px;(quatro cantos) border-radius: 20px 10px;(topo superior esquerdo e canto inferior direito com 20px e topo superior direito e canto inferior esquerdo com 10px;, tambem sendo possivel aplicar em cada canto = border-radius: 10px 25px 8px 19px; por exemplo. border-radius: 10px/30px; horizontal e vertical <.  tambem sendo possivel com porcentagem % exemplo border-radius: 50%; (detalhe ele so vai se tornar circulo se ele for um quadrado perfeito em dimensões por exemplo 200px por 200px.
- bordas com imagem: tem a shorthand que é possivel aplicar varias propriedades na mesma linha também. Suas propriedades são: border-image-source: url('.../'); (para funcionar anteriormente deve-se ter declarado um border). Também da para usar linear gradiente e por ai vai de cores, exemplo: border-image-source: linear-gradient(red, blue);. É possivel fatiar a imagem com slice por regioes, top left,bottom,top,center, fill etc.. border-image-slice: 30; por exemplo, importante usar em conjunto com o border-image-repeat: repeat; temos tambem o border-image-width: 10px; para mudar o tamanho da largura da imagem da borda. border-image-repeat: stretch; (estica as laterais), border-image-repeat: round; (redimensiona sem cortar a imagem), border-image-repeat: space; (adiciona espaços). border-image-outset: 30px; (faz com que a borda se afaste 30px do elemento nesse exemplo). E fazendo a shorthand, por exemplo: border-image: url('...') ou linear gradient(que ambos seriam o border-image-source) em seguida 159(slice) / 40px(width) / 2(outset) round(repeat), então ficaria = border-image: url('../') 159 / 40px / 2 round;
## FONTES
- Fontes serifadas (serif) São compostas por pequenos traços e prolongamentos que ficam no fim de cada letra, conhecido como serifas, exemplo: Times New Roman e Georgia. Outro tipo de fontes que nos temops são as fontes sem serifa (sans-serif), exemplo: arial. Fontes enfeitadas(display) as fontes dessa familia são consideradas tipografias comemorativas ou enfeitadas, muito usadas em textos curtos e pontos para chamar atenção, arte, exemplo: Sabrva Typeface, High Mount. Fontes manuscritas(handwriting) são fontes que se assemelham com a erscrita a mão, conhecidas como manuscritas ou cursivas, traz uma sensação de humanização da escrita, exemplo: scriptina regular, journal, jenna sue. Fontes monoespaçadas(monospace) tem como caracteristicas os caracteres que ocupam a mesma largura, exemplo: monaco, crystal, rayze. Um bom local para acessar essas fontes é o Google Fonts, Awesome Fonts entre outros.
- font-family essa é a propriedade que permite definir qual fonte nos queremos aplicar nos textos, definindo uma fonte especifica ou um, grupo de familia de fontes, exemplos: font-family: sans-serif; , font-family: cursive; font-family: "Times New Roman", "Arial", sans-serif; (ele tentara aplicar a times new roman, caso de algum erro aplicará a Arial, se mesmo assim nao aplicar, ira aplicar a sans-serif.
- @Font-Face permite aplicar uma fonte personalizada que nao está pré instalada no nosso sistema operacional, exemplos: @font-face {  (nomeia a fonte que estamos criando) font-family: Roboto;  
 src: local()(procura na propia maquina do usuario para ver se ja tem a fonte instalada, caso nao esteja ele vai para o url >), url("../fonts/Roboto-Regular.ttf");(neste url eu posso pegar de um servidor externo, ou direto de um arquivo meu já baixado)  }.
Tesmo a propriedade font-weight: normal; é a espessura do letra, tendo o normal, bold, e lighter, tambem utilizando numeros de 100 a 1000.
- @import url() é outra maneira de importar letras de um servidor externo ou local, exemplo: @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;700&display=swap');. Também é possivel pela tag link.
- font-size: essa propriedade define o tamanho da fonte, exemplos: font-size: 20px; font-size: xx-small; / x-small; / small; / medium; / large; / x-large; / xx-large;. O elemento filho costuma pegar o font-size do elemento pai, e dois atributos para trabalhar com elementos filhos pode ser o font-size: smaller; ou font-size: larger; onde ele se baseia no pai para mudar o tamanho do elemento filho.
- font-style: essa propriedade define o estilo da fonte, sendo eses estilos: normal, italic e oblique.
- font-variant: essa propriedade pode definir se nosso texto deve ser exibido em formato versalete (small caps), torna o texto em letras maiúsculas porem diminui o tamanho das letras.
- font-stretch: deixa o texto mais estreito, condensado, ou mais largo expandido, essa propriedade só funciona se a fonte escolhida tiver o suporte para ela. Tendo como atributos: ultra-condensed, extra-condensed, semi-condensed, expanded, extra-expanded, ultra-expanded.
- font-weight: define a largura da fonte.
- line-height: geralmente por padrao o seu atributo tem 1.2; essa propriedade define a altura da nossa linha. Da pra usar porcentagem tambem, o ideal é acima de 1.5 ou 100%.
- font é a propriedade resumida shortcut, em uma unica linha de codigo, exemplo: font: 20px(tamanho da fonte) Arial, sans-serif italic small-caps bold (line-height)2; (talvez tenha que mudar a ordem dos elementos).
 ## TEXTOS
- text-transform: Essa propriedade é responsavél por definir quais caracteres vão estar em maiúsculo, minusculo, etc.. exemplo: text-transform: none;(padrao nao altera nada), text-transform: capitalize; ele vai transformar o primeiro caracter de cada palavra em caixa alto, text-transform: uppercase; transforma o texto totalmente em caixa alto, text-transform: lowercase; tudo em minúsculo. inherit(para herdar do elemento pai) e initial para setar o valor padrão.
- text-align: Essa propriedade é responsavél por alinhar o nosso texto no nosso elemento, exemplos: text-align: left; / right / center / justify(evita sobrar espaços laterais).
- text-decoration: Adiciona ou remove linhas no nosso texto, sejam linhas no meio, em cima ou em baixo. exemplos: text-decoration: none; , text-decoration: underline; , text-decoration: line-through; , text-decoration: overline;.  Text-decoration é um shortcut, então algumas propriedades separadas são: text-decoration-line: underline;(define a linha igual citado acima) , text-decoration-style: solid; / double / dotted / dashed / wavy. text-decoration-color: red; define a cor da linha. text-decoration-thickness: determina a espessura da linha, ex: text-decoration-thickness: 5px;
- text-indent: define o recuo da primeira linha do nosso texto, exemplo: text-indent: 10px; text-indent: -5px;.
- letter-spacing: adiciona um espaçamento entre cada caracter do seu texto, espaçamento entre letras. exemplo: letter-spacing: 5px; letter-spacing: -2px;
- word-spacing: adiciona um espaçamento entre cada palavra do seu texto. exemplo: word-spacing: 5px; word-spacing: -2px;
- white-space: define como os espaços em branco do texto de um determinado elemento é tratado. white-space: normal; white-space: nowrap;(o conteudo do nosso elemento nao é quebrado, entao o texto se mantem em apenas uma linha, ignorando o limite do width tambem. white-space: pre;(preserva todos os espaços em branco e aceita as quebras de linha, porém ultrapassa a largura maxima tambem. white-space: pre-line;(respeita as quebras de linha e quebra quando atinge o limite do container). white-space: pre-warp;(preserva os espaços em branco, quebra o texto nas quebras de linha e no limite do elemento tambem). white-space: break-spaces;(preserva os espaços em branco, faz as quebras de linha, e ele quebra os espaços exedentes na proxima linha para fazer caber no nosso elemento.
- word-wrap: essa propriedade permite definir quando uma palavra é muito grande para caber em uma linha, se ela será quebrada em qualquer caractere para que uma parte dela fique na linha e o restante na proxima, ou se não, toda palavra deve ficar na mesma linha e ultrapssar os limites que definimos para o elemento. word-wrap: normal;(padrão, continua na mesma linha ultrapassando os limites do nosso elemento). word-wrap: break-word;(quebra a palavra para respeitar o elemento).
- word-break: essa propriedade permite definir quebras de linha. word-break: normal;(padrao, espera terminar a palavra ou hífen para quebrar a linha). word-break: break-all;(ele começa a imprimir a palavra que ultrapassaria o container, sem fazer a quebra de linha anterior). word-break: keep-all;(esse texto nao deve quebrar a linha mesmo que a palavra ultrapasse os limites do container, se for um idioma como japones, coreano, chines, pro resto das linguas é aplicado o word-break: normal;.
- writing-mode: Define a orientação do texto(vertical ou horizontal), é bastante utilizada com idiomas que costumam ser lidos verticalmente, da direita para esquerda. writing-mode: horizontal-tb;(valor padrão, esquerda para direita e a proxima linha sempre é posicionada abaixo da anterior). writing-mode: vertical-rl;(da direita para esquerda verticalmente, e a proxima linha é adicionada verticalmente tambem, a esquerda da linha anterior). writing-mode: vertical-lr;(verticalmente tambem, porém as proximas linhas sao adicionadas a direita da anterior).
- text-overflow: clip;(padrao). text-overflow: ellipsis;(adiciona reticencias ao final do texto, sinalizando que há mais conteudo escondido. text-overflow: string; = text-overflow: 'Ver mais >';(mostra o Ver mais > ao final do texto mostrando que ha mais conteudo, detalhe importante funciona apenas no firefox).
- box-shadow: Essa propriedade, aplica uma sombra ao nosso elemento, exemplo utilizando horizontal e vertical = box-shadow: 10px 15px; definindo cor a sombra = box-shadow: 30px 30px red; para melhorar o efeito da sombra deve-se usar o desfoque assim = box-shadow: 30px 30px 10px red;(seria o terceiro valor). Um quarto valor iria definir como a sombra deve ser propagada(aumenta ou diminiu o tamanho da sombra). Para definir uma sombra interna utiliza-se o inset, exemplo: box-shadow: inset 10px 10px 10px red;. É possivel ter varias camadas de sombra, separando por virgula, exemplo = box-shadow: inset 10px 10px 10px red, 20px 20px black;. É possivel aplicar sombras em imagens tambem, para uma utilização com imagens com fundo transparante deve-se utilizar a propriedade filter: drop-shadow(10px 10px 5px gray);.
- text-shadow: adiciona efeitos de sombra nos textos, exemplo: text-shadow: 10px 10px;(horizontal e vertical, pega a cor do texto). Com desfoque e cor = text-shadow: 10px 10px 5px red;
- opacity: define o nivel de opacidade(transparencia) de um elemento, de 0 até 1, sendo 0 o máximo de transparencia e 1 nada de transparencia. Exemplo = opacity: .5;(seria 50%).
- overflow: essa propriedade define como nosso conteúdo deve se comportar caso ele ultrapasse os limites do nosso elemento. overflow: visible;(padrão , fica visivel oque passa do elemento. overflow: hidden;(oque nao couber no elemento será cortado, nao ficara visivel para o usuario, ficara oculto). overflow: scroll;(cria uma barra de scroll para acessar o conteúdo que ultrapassar o elemento. overflow: auto;(cria uma barra scroll tambem, porem a barra de rolagem so vai aparecer caso o conteudo passe do tamanho do elemento). O overflow só funciona com elementos em bloco que tem uma altura definida. Também da para usar somente na vertical ou horizontal, utilizando overflow-y ou overflow-x.
## Redefinindo as propriedades padrões dos navegadores
- Para evitar conflitos com os navegadores, devemos redefinir as configurações dos mesmos, utilizando a tecnica ResetCSS, que cria uma folha de estilos para sobrepor as propriedades que os navegadores colocam por padrão, isso vai ajudar com que o site tenha o mesmo design em todos os navegadores. A forma mais comum é utilizando o seletor universal * { padding: 0; margin: 0; vertical-align: baseline; list-style: none; border: 0; } Na internet voce pode encontrar direntes arquivos que voce pode usar como reset tambem. Indica-se fazer esse reset em uma folha css separada e traze-la para o seu style.css através do @import url('....');.

## NORMALIZE CSS
- o normalize css serve para tirar os estilos padrões dos diversos navegadores, assim evitando problemas com margin, estilos pre definidos entre outros. Então ele é um css que padroniza todo o estilo inicial, fazendo ficar igual nos diversos navegadores. Existem varios tipos, geralmente usamos o CDN que é um servidor disponivel para qualquer pessoa utilizar.
- [CDN NORMALIZE CSS](https://cdnjs.com/libraries/normalize)
- Após acessar o link copie a link tag e cole no seu head no html.


# JAVASCRIPT
## Aprendendo 
```
 - console.log('mensagem'); imprime uma mensagem
 - let variavel = 10; o let cria uma variavel que pode mudar de valor conforme desejado
 - const pi = 3.14; o const cria uma variavel de valor fixo, que nao podera ter seu valor alterado
 - operadores matemáticos = +, -, *, /.
 - operadores condicionais (booleans) = > (maior que), < (menor que), >= (maior ou igual), <= (menor ou igual), ==(igual, que ignora o tipo da variavel, podendo por exemplo ser 0 ou '0', === (igual absoluto, com  o  mesmo tipo de variavel, sem conversão implicita), && (and, e), ! (diferente de), % (resto da divisão, multiplo de).
 - fazendo comentario no código = /* (abrindo) e */ (fechando).
 - console.log(variavel.toFixed(0 a 20)) = o toFixed fixa um numerode casas decimais e arredonda, por exemplo se for passado o valor dois em um numero 36.49787856757 oque seria mostrado para o usuario seria 36.50
 - if (condicao) abre { , codigo, } fecha = (SE) somente executa as linhas de codigo do if SE as condições forem compativeis. else = (SENAO) caso o if nao seja compativel entao executa o else. else if = senao faça esse novo if . ! (negação (senao))
 - function teste() {  } = declara uma funcão de nome teste. invocando a função = teste();. return (retorna um valor).
 - objeto = é uma coleção dinamica de chaves e valor, exemplo const guilherme = { nome: 'Guilherme de lima beraldo', idade: 25 }; e para chamar a idade por exemplo seria guilherme.idade = 24; , tambem da pra deletar uma das caracteristicas por exemplo = delete guilherme.nome . Suas propriedades tambem podem receber funcoes por exemplo = idade: function() { console.log(`Minha idade é ${this.idade}`); } , o THIS significa este, entao estaria pegando o valor de idade DESTA funcao. Também é possivel acessar a propriedade dinamicamente, por exemplo a chamada normal seria console.log(guilherme.nome); e chamando dinamicamente(sem saber o nome do atributo) seria console.log(guilherme['nome']); e mudando seu valor como = guilherme['nome'] = teste; por exemplo.
 - classe = cria uma definicao de como deve ser por exemplo : class Pessoa { nome; idade; } entao as instancias podem utilizar a classe pessoa como paramento, por exemplo : const guilherme = new Pessoa(); guilherme.nome = 'guilherme beralo'; guilherme.idade = 25;
 - constructor = deixa pre definido valores que podem ser obrigatorios por exemplo: (dentro da class) constructor() { this.nome = 'teste'; this.idade = 20; } fazendo assim quando uma nova pessoa for criada ela ja tera o valor nome teste e idade 25 ja pre definidos. tambem podemos exigir que seja informado um parametro, por exemplo: constructor (nome, idade) { this.nome = nome; this.idade = idade; }
- Array (lista) exemplo : const alunos = ['Guilherme', 'Heloisa', 'Marcelo']; que estão na posição Guilherme [0], Heloisa [1], Marcelo [2]. Adicionando mais elementos no final do array(lista) = alunos.push('Valkiria'); , ou alunos[4] = 'Valkiria'; assim aplicando diretamente na posição, e para adicionar ao inicio do array(lista) alunos.unshift('Valkiria'). Também da pra sobrescrever, apagando o elemento que estiver alocado por exemplo : alunos[1] = 'João'; isso faria com que joão sobrescrevece heloisa que estava na posição 1. Removendo itens do final da lista : alunos.pop(); , para ver o elemento que foi removido: console.log(alunos.pop()); e para remover do inicio da lista alunos.shift();. Para remover mais de um item e a partir da posição que eu informar : var pos = 1; var n = 2; var itensRemovidos = vegetais.splice(pos, n);
// Isso é como se faz para remover itens, n define o número de itens a se remover,
// a partir da posição (pos) em direção ao fim da array. console.log(itensRemovidos);
// ['Nabo', 'Rabanete']
Copair um array : var copiar = frutas.slice();.
  . Acessar um item (index) do Array exemplo: var primeiro = frutas[0]; var ultimo = frutas[frutas.length - 1];. Para ver o tamanho do array(lista) = console.log(alunos.length);. Para procurar a posição de um item especifico dentro da array : const pos = frutas.indexOf("Banana"); por exemplo < . Para percorrer o array com For (estrutura de repetição), deve-se criar uma variavel para servir como index que vai ser o controlador do número de repetições a serem feitas na lista por exemplo : for(let i = 0; i < array.lenght; i++) { código } (o i++ é a mesma coisa que fazer i = i + 1, entao ele incrementa 1 no valor do index, fazendo o código seguir executando cada elemento. Separando por virgula conseguimos trabalhar com duas camadas de imagem por exemplo ou mais : background-size: 200px 100px, cover; aplicaria para duas imagens a primeira com 200px 100px e a outra com cover.
- Uma boa pratica é quando for fazer um site começar pela parte mobile, e depois ir aumentando, evitando gerar mais códigos css, entçao mobile first.
- print(`${var}:`); resulta em 2: por exemplo, o ${} permite imprimir uma variavel dentro de um escopo de string, assim concatenando com a string. Detalhe deve se utilizar ` ` em vez de " " ou ' '.
- Para fazer uma herança em javascript utiliza-se o __proto__: atributo; exemplo = const renan = { nome: 'renan', idade: 30, __proto__: pessoa } const pessoa = { genero: 'masculino' }, então um console.log(renan.genero); conseguiria acessar e imprimiria masculino, isso é orientação a protótipo.
## Manipulação de listas
- forEach (para cada): é uma forma de percorrer a lista orientada a funções, percorrendo a lista (semelhante ao for). Exemplo: lista.forEach((value, i, listRef) => { console.log(value, i, listRef); }), considerando a const lista = [1, 2, 3,]; este for each imprimiria: 1 0 [1, 2, 3] 2 1 [1, 2, 3] 3 2 [1, 2, 3]. Detalhe importante, o forEach é um pouco mais lento que o for tradicional, porem com menos codigo, se for trabalhar com uma lista muuuito grande é recomendando utilizar for.
- filter (filtrar): (similar ao forEach) com o filter a gente filtra os elementos que queremos da lista, assim formando uma nova lista sem alterar a lista original. Exemplo: considerando a const lista = [1, 2, 3, 4, 5, 6]; poderiamos fazer por exemplo: const listaDeNumerosPares = lista.filter((element) => { return (element % 2 === 0) }); console.log(lista); console.log(listaDeNumerosPares); este código imprimiria = [1, 2, 3, 4, 5, 6](lista original) [2, 4, 6](nova lista).
- map: o método map é utilizado para converter uma lista em outro objeto por exemplo, uma função que esta com objetivo de tranformação de um elemento em outro. Exemplo: considerando class Pessoa { constructor(nome) { this.name = nome } } e const lista = [new Pessoa('Guilherme'), new Pessoa('Heloisa'), new Pessoa('Renan')]; poderiamos fazer: const listaNomes = lista.map((element, i) => { return `${i} - ${element.name}` }) console.log(listaNomes); imprimiria: ['0 - Guilherme', '1 - Heloisa', '2 - Renan']. Também é posivel tranformar em uma lista HTML, exemplo de return: return ` <li> ${element.name} </li> `.
- reduce: (é utilizado para reduzir a lista a um único valor). Exemplo: considerando const lista = [1, 2, 3, 4, 5, 6]; const somaDosNumeros = lista.reduce((previous, current) => { return previous + current}) console.log(somaDosNumeros); iprimiria: 21 (por trás dos panos oque está acontecendo: 1(previous) + 2(current) = 3, 3(previous) + 3(current) = 6, 6(previous) + 4(current) = 10, 10(previous) + 5(current) = 15, 15(previous) + 6(current) = 21. Então ele percorre a lista e vai somando como um for e no final retorna apenas um elemento que foi o 21. Nós tambem podemos passar um valor inicial como segundo parameto exemplo: lista.reduce((previous, current) => { return previous + current},2(este aqui seria o segundo parametro, o valor inicial)) entao o codigo iniciara assim: 2(previous) + 1(current) = 3, 3(previous) + 2(current) = 5, e assim por diante.
- join: (juntar) ele acrecenta a lista oque for informado entre cada elemento, exemplo: considerando const lista = [1, 2, 3] console.log(lista.join('/')); imprimiria: 1/2/3. Outro exemplo const lista = [1, 2, 3] console.log(lista.join(';')); imprimiria: 1;2;3 .
- Combinando funções de manipulação, utilizando em conjunto, exemplo: considerando const lista = [{nome: 'Guilherme'}, {nome: 'Amanda'}, {nome: 'Rodrigo'}, {nome: 'Andressa'}];  console.log(  lista.map(e => e.nome)  .filter((e) => e.startsWith('A'))  .join('; ') )  isto imprimiria: Amanda; Andressa .
## Assincronimo
- Promises: é uma função assincrona que em algum momento vai devolver um resultado em algum momento, se deu certo ou se deu errado. Exemplo: new Promise((resolve, reject) => { //....... (código) resolve() se esse codigo der certo, reject() se nao der certo. Outro exemplo: const promessaDeNumeroQualquer = new Promise((resolve, reject) => { const numero = parseInt(Math.random() * 100)  resolve(numero) })  promessaDeNumeroQualquer .then((value) => { console.log(value) {) (caso o código de certo faça o console log value) .catch((error) => { console.log(error) }) (caso o código der erro faça o console log erro) .finally(() => { console.log('finalizou') }) (independente de der erro ou dar certo faça console finalizou).
- Await: é uma forma de utilizar as promises mais eficaz e de melhor inerpretação, exemplo(considerando const fs(filesystem) = require('fs') const path = require('path') const filePath = path.resolve(__dirname, 'tarefas.csv'): function buscarArquivo () { const arquivo = await fs.promises.readFile(filePath) const textoDoArquivo = arquivo.toString('utf-8') console.log(textoDoArquivo)  Esse código fara com que imprima o texto que esta no meu arquivo, o await ali significaria (quando eu ler o arquivo mande-o para minha variavel arquivo, então ele espera ler e faz a ação).
 


