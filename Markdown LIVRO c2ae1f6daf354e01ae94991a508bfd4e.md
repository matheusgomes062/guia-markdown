# Markdown LIVRO

# Sobre

Este livro irá abordar os fundamentos de edição de texto em *markdown editor* para que você possa tanto escrever ótimos READ.me's quanto ter uma melhor experiência editando textos!

Irei passar por diversos tópicos, estes sendo:

- O que é Markdown? Como funciona?
- Configuração do ambiente de edição.
- Sintaxe básica.
- Sintaxe avançada.
- Melhores Práticas

Ao ler este livro, você irá desenvolver um texto estilo wiki/READ.me junto comigo de forma a colocar em prática seus conhecimentos. Não só isso, mas iremos abordar também padrões e melhores práticas, assim você poderá sair como um mestre da documentação!

Vamos lá?

# Introdução

Olá! Seja bem vindo!

Me chamo Matheus Gomes e ocasionalmente escrevo abordando temas dos mais diversos assuntos. Utilizei diversas ferramentas durante esse período, porém a ferramenta que mais gostei foi o *markup* *markdown editor.* Eventualmente irei explicar sobre o *markup* e *markdown editor*, porém o que posso dizer agora é que o que me atrai bastante neste markup é que seu uso parece natural, não é necessário muita prática para sair escrevendo. Basta aprender uma dúzia de sintaxes que já é possível fazer um texto muito mais estilizado e coeso.

Se você tem costume de versionar seus projetos no Github é muito possível que já tenha utilizado Markdown, ou até que esteja lendo este livro com a idéia de aprender sobre a "Linguagem do Github".

Eu acredito que hoje não há um livro brasileiro sobre escrita com Markdown, apesar de estar tão inserido na comunidade de desenvolvedores e tão disseminado pelas empresas em suas documentações. É aquela "linguagem" que ninguém sabe ao certo como usa mas acaba usando toda semana. Portanto esse livro seria possivelmente o primeiro no país, e o intuito é ser algo como um guia rápido e ao mesmo tempo um documento profundo e bem documentado sobre o Markdown. 

Ademais, acredito que saber escrever com Markdown te proporciona uma perspectiva diferente sobre o documento, além de fornecer mais liberdade para o usuário poder estilizar o texto como bem entender de forma rápida e prática.

Acredito, assim como [Matt Cone](https://www.mattcone.com/) cita em seu livro "The Markdown Guide", que o  Markdown teve sucesso por ser o ponto de equilíbrio entre simplicidade e poder. Criado em 2004 milhões de pessoas tem utilizado ele para escrever desde notas até mesmo documentos. 

Outro ponto importante a ser mencionado é que este é minha primeira aventura em um livro, não só isso, mas um livro inteiramente escrito em Markdown utilizando diversos softwares de escrita que serão abordados mais a frente. Importante dizer que o livro que me motivou a escrever este foi o "The Markdown Guide" e a página de [John Gruber](https://daringfireball.net/projects/markdown/syntax) sobre o assunto. Teremos também um repositório no github onde o livro estará disponível para fecharmos o ciclo de "um livro sobre markdown escrito em markdown e versionado no github".

Sem mais delongas, vamos lá, primeiramente...

# O que é Markdown? Como funciona?

Criado em 2004 por [John Gruber](https://daringfireball.net/projects/markdown/), Markdown é um linguagem de marcação de texto que adiciona elementos de [formatação em texto simples](https://www.markdownguide.org/getting-started/), sendo uma das linguagens de marcação mais utilizadas no mundo.

Não devemos confundir Markdown com [WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG) ou mesmo algo como *Google Docs* ou *Word*. Isso porque programas como Word ou Google Docs, você clica em botões para mudar frases ou textos. Estas mudanças aparecem imediatamente e são diretamente relacionadas a estes botões. Diferente, o Markdown se baseia em um arquivo de texto formatado para indicar quais palavras e frases devem ser "estilizadas" de outra forma.

Por exemplo, em um documento, padrão Google Docs ou Word que utilizam WYSIWYG, caso  tenhamos o interesse de escrever um texto em negrito (*bold*), teria que clicar na opção de negrito (ou utilizar o comando `Ctrl+b`), em comparação, no Markdown, seria obtido o mesmo resultado adicionando asteriscos antes e após a palavra que se deseja por em negrito, ou seja:  `**esse texto está em negrito**` .

### Visualização

**esse texto está em negrito**

Assim, o  Markdown funciona utilizando de caracteres especiais que são postos antes e/ou depois de determinados blocos de texto para criar a estilização necessária!

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled.png)

Exemplo do Negrito em WYSIWYG

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%201.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%201.png)

Exemplo de Markdown retirado do meu artigo no dev.to

## Mas e por debaixo dos panos?

Por debaixo dos panos o Markdown funciona da seguinte forma:

1. Escrevemos um texto em um arquivo `.md` ou `.markdown`
2. Este arquivo é então lido por um processador de Markdown. Isto é, o aplicativo que utilizaremos para ler ou editar utiliza esse processador para interpretar a linguagem que estamos escrevendo.
3. A aplicação Markdown então irá converter o arquivo Markdown em um documento HTML.
4. Exportando tal arquivo é possível analisar no browser ou até mesmo converter o arquivo para outro formato, como PDF.

O [Typora](https://typora.io/) por exemplo une os passos 1, 2 e 3, assim podemos visualizar a conversão em tempo real!

Apesar da diferença, você irá perceber logo mais a facilidade e rapidez que a marcação Markdown proporciona, basta continuar e acompanhar os exemplos!

> “Um dia encontrarei as palavras certas, e elas serão simples.”
-Jack Kerouac

# Por que utilizar markdown?

Como vimos anteriormente, temos algumas soluções para a marcação de textos com o WYSIWYG, assim, porque deveríamos aprender Markdown se esta solução já resolve?

Vamos listar os pontos do porque devemos aprender Markdown:

- **Markdown pode (e é) utilizado para tudo**. Pessoas utilizam Markdown para criar [sites](https://mkdocs.github.io/mkdocs-basic-theme/),  documentação, anotações, livros (como este), [apresentações](https://marp.app/), mensagens de email, documentação técnica e muito mais. O limite está na criatividade!
- **Markdown é portátil**. Arquivos escritos em Markdown podem ser abertos utilizando quase que qualquer aplicação. Se você não gostar do app que está utilizando para escrever em Markdown, você pode simplesmente importar o arquivo de texto atual para outro aplicativo que atenda melhor as suas necessidades. Eu por exemplo gosto muito de utilizar o [Typora](https://typora.io/), no entanto, eu atualmente tenho escrito no [Notion](https://www.notion.so/) pela praticidade e estilo. A questão é, independente da plataforma o Markdown é universal, ao contrário do documento Word ou Google docs que seguem padrões próprios e necessitam de aplicativos específicos.
- **Markdown é independente.** Qualquer dispositivo ou sistema operacional consegue 'rodar' marcação do tipo Markdown.
- **Markdown é consolidado.** Mesmo que sua aplicação de edição parar de funcionar no futuro, pelo Markdown ser consolidado ainda será possível ler o arquivo. Isto é de extrema importância para quando tratamos de livros, artigos acadêmicos ou   mesmo documentos importantes que precisam ser preservados.
- **Markdown está em todo lugar**. Como dito no primeiro tópico, além de utilizado para tudo, ele está em tudo. Funcionando tanto no [Reddit](https://www.reddit.com/) quanto no [Github](https://github.com/), encontramos o Markdown nas mais diversas plataformas web, sendo possivelmente a linguagem de marcação mais utilizada no mundo (depois do HTML, claro).

Mas vamos lá! 

Primeiramente iremos...

# Configurar o ambiente de edição

Para acompanhar o curso é importante que você utilize um editor de texto que suporte Markdown. Temos diversas opções disponíveis, tanto gratuitas quanto pagas. 

Aqui irei dispor algumas dessas opções:

- [Typora](https://typora.io/)
- [Dillinger](https://dillinger.io/)
- [GhostWriter](https://wereturtle.github.io/ghostwriter/)
- [Zettlr](https://www.zettlr.com/)
- [Notion](http://notion.so)
- [StackEdit](https://stackedit.io/)
- [editor.md](https://pandao.github.io/editor.md/en.html)

Neste livro utilizaremos o Typora por ser *open source* (no momento que escrevo o Typora é **open source**, mas eventualmente ele irá se tornar pago), ou seja, **é gratuito**. Ele também é uma aplicação para Windows, Mac (Beta) e Linux, ou seja, **podemos utilizar em qualquer lugar**. Por fim, escolho o Typora pela **ampla base de usuários**, **simplicidade**, e **leveza** e por ser **possível adicionar temas**!

Portanto, basta baixar e instalar o Typora, ou editor de preferência para podermos iniciar o curso!

> “Escrever é uma forma socialmente aceitável de esquizofrenia.”
― E.L. Doctorow

# Sintaxe Básica

Como o Markdown basicamente converte o que escrevemos para HTML, irei abordar o ensino da linguagem contrapondo e referenciando o HTML. Caso você não saiba sobre HTML, não tem problema, não é necessário saber HTML, mas fica mais fácil para entender caso você saiba sobre. De qualquer forma, esse livro não exige conhecimento prévio de programação!

A apresentação da linguagem será dada da seguinte forma:

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Screen_Shot_2021-07-03_at_17.10.37.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Screen_Shot_2021-07-03_at_17.10.37.png)

Vamos lá.

## Títulos

Para títulos utilizamos a cerquilha (ou infamemente conhecida como jogo da velha) `#` . O título é medido pelo número de vezes que a cerquilha é posta em conjunto, ou seja,  utilizaremos duas cerquilhas para caso queiramos representar um título em `h2`, ou em termos leigos, um título um tanto menor que o título de maior tamanho.

Aqui está algo mais claro e prático:

[Títulos](https://www.notion.so/be2fdda780f24ac7a2620aa8a1f19bae)

## Sintaxe alternativa para Títulos

Existe uma sintaxe alternativa para títulos, pouco usada. Tal sintaxe serve apenas para títulos de nível 1 e 2. Ela funciona da seguinte forma, colocamos o sinal de menos  (`-`) na linha abaixo do título para mostrar o título como título de nível 1. E utilizamos o  sinal  de igual (`=`) na linha abaixo do título para mostrar o título como título de nível 2.

Exemplificando:

[Títulos  (Alternativo)](https://www.notion.so/56f5fe7569284116b486265f5d382ca8)

## Melhores práticas para Títulos

As aplicações geralmente não concordam sobre o espaço entre a cerquilha e o título. Para compatibilidade sempre utilize um espaço entre os dois.

Exemplo:

`# Título com espaço` ✔

`# Título sem espaço` ❌

## Parágrafos

Para criar parágrafos, utilizamos uma linha em branco para separar as linhas de texto.  Não devemos identar os parágrafos com espaços ou *tabs,* pois isso irá representar outra função diferente do parágrafo.

Exemplo:

### Markdown

```bash
1. Estou começando a gostar de escrever com Markdown
2.
3. Acho que irei usar isso daqui pra frente.
```

### HTML

```html
1. <p>Estou começando a gostar de escrever com Markdown</p>
2.
3. <p>Acho que irei usar isso daqui pra frente.</p>
```

### Visualização

Estou começando a gostar de escrever com Markdown

Acho que irei usar isso daqui pra frente.

## Melhores práticas para Parágrafos

A não ser que o parágrafo esteja numa lista, não idente os parágrafos com espaços ou tabs.

`Não utilize tabs ou espaços na frente do seu parágrafos.` ✔

`Deixe as linhas alinhadas a esquerda assim.` ✔

    `Isso pode ocasionar problemas de formatação` ❌

 `E adicionar espaços no começo pode atrapalhar a leitura.` ❌

## Quebra de linha

A quebra de linha é bem simples, basta adicionar dois ou mais espaços no final de uma linha e então apertar enter (return no mac).

Exemplo:

### Markdown

```bash
1. Esta é a primeira linha.  
2. E esta é a segunda linha.
```

### HTML

```html
1. <p>Estou começando a gostar de escrever com Markdown<br />
2. E esta é a segunda linha.</p>
```

### Visualização

Esta é a primeira linha.
E esta é a segunda linha.

## Melhores prática para quebra de linha

Utilizar dois espaços para quebrar linhas pode ser usada em quase todas as aplicações, mas isso é relativamente controverso. Comumente é adicionado dois espaços sem querer no final das linhas. Por essa razão algumas pessoas gostam de utilizar outra opção para quebra de linha. Felizmente existe uma opção apoiada por algumas aplicações Markdown. Tal opção é o uso da tag <br> no final da linha.

Existem algumas aplicações que possibilitam o uso da barra invertida para quebrar linhas, porém eu não posso recomendar seu uso, visto que:

1. Não são todas que adotam essa funcionalidade.
2. Não é uma boa opção de compatibilidade.

E existem outras aplicações de Markdown que não necessitam de nada no final da linha, apenas apertar Enter quebra a linha.

Exemplo:

`Primeira linha com dois espaços depois.` ✔
`E sua próxima linha.`

---

`Primeira linha com uma barra invertida depois.\` ❌
`E sua próxima linha.`

---

`Linha com tag HTML de break row.<br>` ✔
`E sua próxima linha.`

---

`Linha sem nada depois, só um enter.
E sua próxima linha.`

## Destaque

No caso, destaques para **negrito** e *itálico.*

### Negrito

Adicionar um texto em negrito exige dois asteriscos (`*`) antes e após o texto selecionado.

Da seguinte forma:

### Markdown

```bash
1. Vou dar ênfase **nisso**.
```

### HTML

```html
1. Vou dar ênfase <strong>nisso</strong>.
```

### Visualização

Vou dar ênfase **nisso.**

## Melhores práticas para Destaque - Negrito

Apesar de não haver concordância entre a melhor prática para o uso de negrito no meio de palavras, acredito que utilizar asteriscos é melhor do que utilizar sublinhados, pois aparentar dar mais ênfase e melhora a compatibilidade.

`Para**lele**pípedo.` ✔

`Para__lele__pípedo.` ❌

### Itálico

Para itálico utilizamos o mesmo conceito, porém ao invés de adicionar dois asteriscos utilizamos um *underline* (Símbolo de sublinhado `_`)*.*

Da seguinte forma:

### Markdown

```bash
1. Michael Jackson dançando fica estilo _itálico_.
```

### HTML

```html
1. Michael Jackson dançando fica estilo <em>itálico</em>.
```

### Visualização

1. Michael Jackson dançando fica estilo *itálico*.

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%202.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%202.png)

Michael Jackson modo itálico.

## Melhores práticas para Destaque - Itálico

Apesar de não haver concordância entre a melhor prática para o uso de itálico no meio de palavras, acredito que utilizar asteriscos é melhor do que utilizar sublinhados, pois aparentar dar mais ênfase e melhora a compatibilidade..

`Bor*bo*leta.` ✔

`Bor_bo_leta.` ❌

## Destaque com sintaxe alternativa

Existe uma outra forma, talvez menos usual de produzir os mesmos destaques. Vejamos como...

### Negrito (Alternativo)

Da mesma forma que utilizamos dois asteriscos para transformar o texto em negrito nós podemos utilizar dois *underlines* para poder obter o mesmo efeito.

### Markdown

```bash
1. Vou dar ênfase __nisso__.
```

### HTML

```html
1. Vou dar ênfase <strong>nisso</strong>.
```

### Visualização

Vou dar ênfase **nisso.**

### Itálico (Alternativo)

Seguindo a mesma proposta, podemos obter o mesmo resultado de itálico utilizando apenas um asterisco de cada lado.

### Markdown

```bash
1. Michael Jackson dançando fica estilo *itálico*.
```

### HTML

```html
1. Michael Jackson dançando fica estilo <em>itálico</em>.
```

### Visualização

1. Michael Jackson dançando fica estilo *itálico*.

## Negrito e itálico

Para dar destaque em um texto com negrito e itálico ao mesmo tempo basta adicionar 3 asteriscos ou 3 underlines antes e depois da palavra ou frase. Para colocar uma palavra em negrito e itálico no meio de uma palavra basta adicionar 3 asteriscos sem espaços em volta das letras.

Exemplo:

### Markdown

```bash
***Texto*** importante.
___Texto___ importante.
__*Texto*__ importante.
**_Texto_** importante.
Palavra ***importante*** no texto.
```

### HTML

```html
<strong><em>Texto</em></strong> importante.
Palavra <strong><em>importante</em></strong> no texto.
```

### Visualização

***Texto*** importante.
Palavra ***importante*** no texto.

## Melhores práticas Negrito e Itálico

Para a utilização dos dois seguimos a mesma ideia de antes, ao utilizar no meio de uma sentença ou palavra, prefira utilizar os asteriscos, pois sua compatibilidade é maior.

`Bor***bo***leta.` ✔

`Bor___bo___leta.` ❌

## Citação

Para criar citações basta adicionar o símbolo de "maior que" (`>`) na frente do parágrafo desejado.

### Markdown

```bash
> “You only live once, but if you do it right, once is enough.”
```

### HTML

```html
<blockquote>
	<p>“You only live once, but if you do it right, once is enough.”</p>
</blockquote>
```

### Visualização

> “You only live once, but if you do it right, once is enough.”

## Citação com múltiplos parágrafos

Podemos também adicionar parágrafos nas citações. Para isso adicionamos um "maior que" nas linhas vazias entre os parágrafos.

### Markdown

```bash
> “You only live once, but if you do it right, once is enough.”
>
> - Mae West
```

### HTML

```html
<blockquote>
	<p>“You only live once, but if you do it right, once is enough.”</p>
	<p>- Mae West </p>
</blockquote>
```

### Visualização

> “You only live once, but if you do it right, once is enough.”
- Mae West

## Citações aninhadas

As citações podem ser aninhadas, para isso adicione duas vezes o símbolo de citação (`>>`) antes do parágrafo desejado.

### Markdown

```bash
> Parágrafo padrão
>
>> Parágrafo aninhado
```

### HTML

```html
<blockquote>
	<p>Parágrafo padrão</p>
	<blockquote>
		<p>Parágrafo aninhado</p>
	</blockquote>
</blockquote>
```

### Visualização

Parágrafo padrão

> Parágrafo aninhado

## Citações com outros elementos

A versatilidade no markdown é bem grande, aqui demonstramos como utilizar outras características do markdown no campo de citações.

### Markdown

```bash
> ##### Cyberpunk 2077 é um jogo fantástico!
>
> - A história é incrível.
> - Gráficos impressionantes.
>
>  *Vale muito* a pena **jogar**!.
```

### HTML

```html
<blockquote>
	<h5>Cyberpunk 2077 é um jogo fantástico!</h5>
	<ul>
		<li>A história é incrível.</li>
		<li>Gráficos impressionantes.</li>
	</ul>
	<p><em>Vale muito</em> a pena <strong>jogar</strong>.</p>
</blockquote>
```

### Visualização

> Cyberpunk 2077 é um jogo fantástico!A história é incrível.Gráficos impressionantes.Vale muito a pena jogar!.

## Listas

É possível organizar seus itens em listas ordenadas e não ordenadas.

### Listas ordenadas

Para criar listas ordenadas, adicione números seguido de um ponto para cada item da linha. Os números não precisam estar em ordem numérica, mas sempre devem começar com o número 1.

### Markdown

```markdown
1. Primeiro item
2. Segundo item
3. Terceiro item
```

### HTML

```html
<ol>
	<li>Primeiro item </li>
	<li>Segundo item </li>
	<li>Terceiro item </li>
</ol>
```

### Visualização

1. Primeiro item
2. Segundo item
3. Terceiro item

## Listas aninhadas

Para alinhar uma lista dentro de uma lista ordenada, identamos os items 4 espaços para direita ou um *tab.*

### Markdown

```markdown
1. Primeiro item
2. Segundo item
	1. Item 1 dentro do segundo
	2. Item 2 dentro do segundo
3. Terceiro item
```

### HTML

```html
<ol>
	<li>Primeiro item </li>
	<li>Segundo item </li>
	<ol>
		<li>Item 1 dentro do segundo </li>
		<li>Item 2 dentro do segundo </li>
	</ol>
	<li>Terceiro item </li>
</ol>
```

### Visualização

1. Primeiro item
2. Segundo item
    1. Item 1 dentro do segundo
    2. Item 2 dentro do segundo
3. Terceiro item

## Listas não ordenadas

Para criar listas não ordenadas, adicionamos traços (-), asteríscos (*), ou sinais de mais (+) na frente das linhas dos items.

### Markdown

```markdown
- Primeiro item
- Segundo item
- Terceiro item

* Primeiro item
* Segundo item
* Terceiro item

* Primeiro item
- Segundo item
* Terceiro item
```

### HTML

```html
<ul>
	<li>Primeiro item </li>
	<li>Segundo item </li>
	<li>Terceiro item </li>
</ul>
```

### Visualização

- Primeiro item
- Segundo item
- Terceiro item

## Aninhando items de uma lista não ordenada

Para aninhar items dentro de uma lista não ordenada, identamos os seus items quatro espaços para direita ou um *tab.*

### Markdown

```markdown
- Primeiro item
- Segundo item
	- Item aninhado
	- Item aninhado
- Terceiro item

* Primeiro item
* Segundo item
	* Item aninhado
	* Item aninhado
* Terceiro item

* Primeiro item
- Segundo item
	* Item aninhado
	- Item aninhado
* Terceiro item
```

### HTML

```html
<ul>
	<li>Primeiro item </li>
	<li>Segundo item </li>
	<ol>
		<li>Item aninhado </li>
		<li>Item aninhado </li>
	</ol>
	<li>Terceiro item </li>
</ul>
```

### Visualização

- Primeiro item
- Segundo item
    - Item aninhado
    - Item aninhado
- Terceiro item

## Adicionando elementos na lista

Para adicionar outro elemento na lista enquanto preserva a lista em si, indentamos o elemento quatro espaços para direita ou um *tab.* Veja os exemplos:

### Adicionando parágrafos

### Markdown

```markdown
- Primeiro item
- Segundo item
	Parágrafo que adicionei no meio da lista
- Terceiro item

* Primeiro item
* Segundo item
	Parágrafo que adicionei no meio da lista
* Terceiro item

* Primeiro item
- Segundo item
	Parágrafo que adicionei no meio da lista
* Terceiro item
```

### HTML

```html
<ul>
	<li>Primeiro item </li>
	<li>Segundo item 
		<p>Parágrafo que adicionei no meio da lista </p>
	</li>
	<li>Terceiro item </li>
</ul>
```

### Visualização

- Primeiro item
- Segundo item

    Parágrafo que adicionei no meio da lista

- Terceiro item

### Adicionando bloco de citações

### Markdown

```markdown
- Primeiro item
- Segundo item
	> Bloco de citação que adicionei no meio da lista
- Terceiro item

* Primeiro item
* Segundo item
	> Bloco de citação que adicionei no meio da lista
* Terceiro item

* Primeiro item
- Segundo item
	> Bloco de citação que adicionei no meio da lista
* Terceiro item
```

### HTML

```html
<ul>
	<li>Primeiro item </li>
	<li>Segundo item
		<blockquote>
			<p>Bloco de citação que adicionei no meio da lista </p>
		</blockquote>
	</li>
	<li>Terceiro item </li>
</ul>
```

### Visualização

- Primeiro item
- Segundo item

    > Bloco de citação que adicionei no meio da lista

- Terceiro item

### Adicionando Bloco de código

Blocos de código são geralmente indentados quatro espaços para direita ou um *tab.* Quando estão em uma lista no entanto, eles são indentados 8 espaços para direita ou 2 *tabs.*

### Markdown

```markdown
- Primeiro passo
- Segundo passo
		<html>
			<head>
				<title>Teste</title>
			</head>
- Terceiro passo

* Primeiro passo
* Segundo passo
		<html>
				<head>
					<title>Teste</title>
				</head>
* Terceiro passo

* Primeiro passo
- Segundo passo
		<html>
			<head>
				<title>Teste</title>
			</head>
* Terceiro passo
```

### HTML

```html
<o>
	<li><p>Primeiro passo</p></li>
	<li><p>Segundo passo</p>
		<pre><code>&lt;html&gt;
			&lt;head&gt;
				&lt;title&gt;Test&lt;/title&gt;
			&lt;/head&gt;
		</code></pre>
	</li>
	<li><p>Terceiro item</p></li>
</o>
```

### Visualização

- Primeiro passo
- Segundo passo

    ```html
    <html>
    	<head>
    		<title>Test</title>
    	</head>
    ```

- Terceiro passo

### Adicionar imagens em listas

Da mesma forma é possível adicionar imagens no meio das listas sem de fato interromper a lista em si.

### Markdown

```markdown
- Primeiro passo
- Segundo passo
		![Exemplo do segundo passo](images/rickroll.png)
- Terceiro passo

* Primeiro passo
* Segundo passo
		![Exemplo do segundo passo](images/rickroll.png)
* Terceiro passo

* Primeiro passo
- Segundo passo
		![Exemplo do segundo passo](images/rickroll.png)
* Terceiro passo
```

### HTML

```html
<o>
	<li><p>Primeiro passo</p></li>
	<li><p>Segundo passo</p>
		<p>
			<img src="images/rickroll.png" alt=rickroll />
		</p>
	</li>
	<li><p>Terceiro item</p></li>
</o>
```

### Visualização

- Primeiro passo
- Segundo passo

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%203.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%203.png)

rickroll

- Terceiro passo

## Código

Para mostrar que determinada frase ou palavra é um código, coloque ela entre acentos (`).

### Markdown

```markdown
Para iniciar o projeto utilize o comando `yarn start`
```

### HTML

```html
Para iniciar o projeto utilize o comando <code>yarn start</code>
```

### Visualização

Para iniciar o projeto utilize o comando `yarn start`

### Como utilizar acentos dentro de códigos markdown

Se a palavra ou frase que você quer escrever tem códigos com um ou mais acentos, você pode ignorar eles encapsulando-os em aspas duplas (").

### Markdown

```markdown
``É possível utilizar `código` dentro do seu arquivo Markdown``
```

### HTML

```html
<code>É possível utilizar `código` dentro do seu arquivo Markdown</code>
```

### Visualização

```html
É possível utilizar `código` dentro do seu arquivo Markdown
```

### Bloco de códigos

Para criar bloco de códigos, indente cada linha do bloco para pelo menos quatro espaços para frente ou um *tab.*

### Markdown

```markdown
	<html>
		<head>
		</head>
	</html>
```

### HTML

```html
<pre>
	<code>
		&lt;html&gt;
			&lt;head&gt;
			&lt;/head&gt;
		&lt;/html&gt;
	</code>
</pre>
```

### Visualização

```html
<html>
	<head>
	</head>
</html>
```

## Linhas horizontais

Para criar linhas horizontais utilize três asteríscos(***), traços(—-), ou sublinhado(___) em uma linha exclusiva para eles.

### Markdown

```markdown
***

---

___________________
```

### HTML

```html
<hr />

<hr />

<hr />
```

### Visualização

---

### Melhores práticas para linhas horizontais

Para compatibilidade, coloque linhas vazias antes e depois das linhas horizontais.

### Markdown

```markdown
Jeito correto ✅
Linha vazia abaixo

***

Linha vazia acima
```

### Markdown

```markdown
Jeito impróprio ❌
***
Não faça isso!
```

## Links

Para criar links é um pouco mais complexo, utilize o texto do link em colchetes (exemplo: [Uncle Bob]) e então coloque logo em seguida a URL entre parenteses (exemplo: ([http://cleancoder.com](http://cleancoder.com/products))).

### Markdown

```markdown
Acesse o [site]([http://cleancoder.com](http://cleancoder.com/products)) do Uncle Bob!
```

### HTML

```html
Acesse o <a href="[http://cleancoder.com](http://cleancoder.com/products)">site</a> do Uncle Bob!
```

### Visualização

Acesse o [site](http://cleancoder.com) do Uncle Bob!

### Adicionando Títulos para links

É possível adicionar títulos para links. Eles apareceram como uma *tooltip* quando o usuário passar o mouse em cima do link. Para adicionar um título é bem simples, basta colocar o título entre parenteses depois da URL.

### Markdown

```markdown
Acesse o [site]([http://cleancoder.com](http://cleancoder.com/products) "código limpo!") do Uncle Bob!
```

### HTML

```html
Acesse o <a href="[http://cleancoder.com](http://cleancoder.com/products)" title="código limpo!">site</a> do Uncle Bob!
```

### Visualização

Acesse o [site](http://cleancoder.com) do Uncle Bob!

### Transformar URL ou email em links clicáveis

Para transformar urls ou emails em links clicáveis de forma prática e fácil basta colocar os links e emails dentro de colchete angulares (< e >).

### Markdown

```markdown
Meu email é <matheusgomes062@gmail.com>
e eu recomendo esse site <https://github.com/>
```

### HTML

```html
Meu email é <a href="matheusgomes062@gmail.com">matheusgomes062@gmail.com</a>
e eu recomendo esse site <a href="https://github.com/">https://github.com/</a>
```

### Visualização

Meu email é matheusgomes062@gmail.com
e eu recomendo esse site [https://github.com/](https://github.com/)

### Formatação de links

Para colocar seus links em itálico ou negrito adicione asteríscos antes ou depois dos colchetes e parenteses. Para transformar o seu link em código, coloque acento nos colchetes.

### Markdown

```markdown
Eu amo e a apoio **[Humble Bundle](https://www.humblebundle.com/)**
Essa é a parte do *[Humble Bundle](https://www.humblebundle.com/)*.
Veja a seção no [`código`](#code).
```

### HTML

```html
Eu amo e a apoio <strong><a href="https://www.humblebundle.com/">Humble Bundle</a></strong>
Essa é a parte do <em><a href="https://www.humblebundle.com/">Humble Bundle</a></em>.
Veja a seção no <a href="#code"><code>code</code></a>.
```

### Visualização

Eu amo e a apoio **[Humble Bundle](https://www.humblebundle.com/)**
Essa é a parte do *[Humble Bundle](https://www.humblebundle.com/)*.
Veja a seção no `[código](https://www.youtube.com/watch?v=dQw4w9WgXcQ)`

## Links de referência de estilo

Links de referência de estilo (em inglês: Reference-style links) é um tipo especial de link que torna mostrar URLs mais fácil de ler em Markdown. Esses tipos de link utilizam dois conjuntos de colchetes.

### Formatando a primeira parte do link

A primeira parte de um link de referência de estilo é formatado com dois conjuntos de colchetes. O primeiro conjunto engloba o texto que aparece como "linkado". O segundo engloba o rótulo que será usado para apontar o link que você está guardando em alguma parte do documento.

Apesar de não ser necessário, você pode incluir um espaço entre o primeiro e o segundo conjunto de colchetes. E o título do segundo conjunto de colchetes não é case sensitivo e pode incluir letras, números, espaços e pontuações.

Isso significa que os seguintes formatos são relativamente equivalentes a primeira parte do link:

- [bola-de-sinuca][1]
- [bola-de-sinuca] [1]
- [bola-de-sinuca][a]
- [bola-de-sinuca] [A]

### Formatando a Segunda Parte do Link

A segunda parte da referência é formatada utilizando os seguintes atributos:

1. O rótulo, em colchetes, seguido imediatamente por dois pontos e por pelo menos um espaço.
    1. Exemplo: [rótulo]: 
    2. A URL do link, no qual você pode encapsular por colchetes angulares (< >).
    3. Um título opcional para o link, no qual você pode encapsular em aspas duplas, aspas simples ou parênteses.

Isso significa que os exemplos abaixo são relativamente equivalentes pela segunda parte do link:

- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle)
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle•[hobbit-hole]:](https://en.wikipedia.org/wiki/Hobbit#Lifestyle%E2%80%A2%5Bhobbit-hole%5D:) [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) "Hobbitlifestyles"
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) 'Hobbitlifestyles'
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) (Hobbitlifestyles)
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) "Hobbitlifestyles"
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) 'Hobbitlifestyles'
- [hobbit-hole]: [https://en.wikipedia.org/wiki/Hobbit#Lifestyle](https://en.wikipedia.org/wiki/Hobbit#Lifestyle) (Hobbitlifestyles)

Você pode colocar a segunda parte do link em qualquer lugar do seu documento Markdown. Algumas pessoas colocam eles imediatamente depois do parágrafo no qual eles aparecem, enquanto outras pessoas colocam eles no final do documento em formato de notas finais ou notas de rodapé.

### Juntando o que aprendemos com links

Vamos dizer que você quer adicionar uma URL como um link padrão de URL em um paragrafo que se assemelha a este:

### Markdown

```markdown
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet h\
ole, filled with the ends of worms and an oozy smell, nor yet a dry, ba\
re, sandy hole with nothing in it to sit down on or to eat: it was a [h\
obbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit life\
styles"), and that means comfort.
```

### Markdown

```markdown
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet h\
ole, filled with the ends of worms and an oozy smell, nor yet a dry, ba\
re, sandy hole with nothing in it to sit down on or to eat: it was a [h\
obbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyle\
s"
```

### HTML

```html
<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle"title="Hobbit \
lifestyles">hobbit-hole</a>
```

### Visualização

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle), and that means comfort.

### Melhores práticas com links

Como algumas aplicações markdowns não concordam entre si em como lidar com espaços no meio de uma URL, iremos utilizar %20 ao invés de espaços para melhor compatibilidade de URLs.

### Markdown

```markdown
Faça isso! ✅

[link](https://www.example.com/my%20great%20page)
```

### Markdown

```markdown
Evite isso! ❌

[link](https://www.example.com/my great page)
```

## Imagens

Para adicionar uma imagem, adicione um ponto de exclamação (!), Seguido do texto alternativo entre colchetes e a imagem do URL entre parênteses.

### Markdown

```markdown
![Philadelphia's Magic Gardens. This place was so cool!](images/philly-\
magic-garden.png "Philadelphia's Magic Gardens")
```

### HTML

```html
<img src="images/philly-magic-garden.png" alt="Philadelphia's Magic Gar\
dens. This place was so cool!"title="Philadelphia's Magic Gardens"/>
```

### Visualização

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%204.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Untitled%204.png)

Philadelphia's Magic Gardens. This place was so cool!

### Imagens com links

Para adicionar um link a uma imagem, coloque o Markdown da imagem entre colchetes e, em seguida, adicione o link entre parênteses.

### Markdown

```markdown
[![An old rock in the desert](images/shiprock.jpg)](https://en.wikipedi\
a.org/wiki/Shiprock)
```

### HTML

```html
<a href="https://en.wikipedia.org/wiki/Shiprock"><img src="images/shipr\
ock.jpg"alt="An old rock in the desert"></a>
```

## Escapando caracteres

Para exibir um caractere literal que de outra forma seria usado para formatar texto em um documento Markdown, adicione uma barra invertida (\) na frente do caractere.

### Markdown

```markdown
\* Without the backslash, this would be a bullet in an unordered list.
```

### HTML

```html
* Without the backslash, this would be a bullet in an unordered list.
```

### Visualização

Without the backslash, this would be a bullet in an unordered list.

### Caracteres que é possível escapar

Você pode usar uma barra invertida para escapar dos caracteres a seguir.

[Sintax básica](https://www.notion.so/fb28ad6153dd41e08b3a3d3c2dec85ad)

pra não esquecer quais são:

![Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Screen_Shot_2021-06-22_at_21.48.27.png](Markdown%20LIVRO%20c2ae1f6daf354e01ae94991a508bfd4e/Screen_Shot_2021-06-22_at_21.48.27.png)

## HTML

Muitos aplicativos Markdown permitem que você use tags HTML no texto Markdown formatado. Isso é útil se você preferir certas tags HTML à sintaxe do Markdown. Por exemplo, algumas pessoas acham mais fácil usar tags HTML para imagens. Usar HTML também é útil quando você precisa alterar os atributos de um elemento, como especificar a cor do texto ou alterar a largura de uma imagem. Para usar HTML, coloque as marcas no texto do arquivo formatado em Markdown.

### Markdown

```markdown
This **word** is bold. This <em>word</em> is italic.
```

### HTML

```html
This <strong>word</strong> is bold. This <em>word</em> is italic.
```

### Visualização

This **word** is bold. This *word* is italic.

### HTML melhores práticas

Por razões de segurança, nem todos os aplicativos Markdown suportam HTML em documentos Markdown. Em caso de dúvida, verifique a documentação do aplicativo Markdown. Alguns aplicativos suportam apenas um subconjunto de tags HTML. 

Use linhas em branco para separar elementos HTML de nível de bloco como `<div>`, `<table>`, `<pre>` e `<p>` dos arredores contente. Tente não recuar as tags com tabulações ou espaços, o que pode interferir na formatação. 

Você não pode usar a sintaxe do Markdown em HTML tags de nível de bloco lateral. Por exemplo, `<p> itálico e ** negrito ** </p>` não funcionam.

## Sintax extendida

A sintaxe básica delineada no documento de design original de John Gruber adicionou muitos dos elementos necessários no dia-a-dia, mas não foi o suficiente para algumas pessoas. É aí que entra a sintaxe estendida. 

Vários indivíduos e organizações assumiram a responsabilidade de estender o sintaxe básica adicionando elementos adicionais como tabelas, blocos de código, realce de sintaxe, link automático de URL e notas de rodapé. Esses elementos podem ser ativados usando uma linguagem de marcação leve que se baseia na sintaxe Markdown básica ou adicionando uma extensão a um processador Markdown compatível. 

### Disponibilidade

Nem todos os aplicativos Markdown oferecem suporte a elementos de sintaxe estendidos. Você precisará verificar se a linguagem de marcação leve que seu aplicativo está usando suporta ou não os elementos de sintaxe estendidos que você deseja usar. Do contrário, ainda pode ser possível habilitar extensões em seu processador Markdown. 

### Linguagens de marcação leves

Existem várias linguagens de marcação leves que são superconjuntos de Markdown. Elas incluem a sintaxe básica de Gruber e a baseiam na adição de elementos adicionais como tabelas, blocos de código, realce de sintaxe , Link automático de URL e notas de rodapé. Muitos dos aplicativos Markdown mais populares usam uma das seguintes linguagens de marcação leve: 

- CommonMark
- GitHub Flavored Markdown (GFM)
- Markdown Extra
- MultiMarkdown
- R Markdown

### Processadores Markdown

Existem dezenas de processadores Markdown disponíveis. Muitos deles permitem que você adicione extensões que permitem elementos de sintaxe estendidos. Verifique a documentação do seu processador para obter mais informações.

## Tabelas

Para adicionar uma tabela, use três ou mais hifens (---) para criar o cabeçalho de cada coluna e use barras verticais (|) para separar cada coluna. Você pode opcionalmente adicionar tubos em qualquer extremidade da tabela.

### Markdown

```markdown
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

### HTML

```html
<table>
	<thead>
		<tr class="header">
			<th>Sintax</th>
			<th>Descrição</th>
		</tr>
	</thead>
	<tbody>
		<tr class="odd">
			<td>Header</td>
			<td>Título</td>
		</tr>
		<tr class="even">
			<td>Parágrafo</td>
			<td>Texto</td>
		</tr>
	</tbody>
</table>
```

### Visualização

[Untitled](https://www.notion.so/6ecaa19253e34d899b3f268ca7e4161e)

### Alinhamento

Você pode alinhar o texto nas colunas à esquerda, à direita ou ao centro adicionando dois pontos (:) à esquerda, à direita ou em ambos os lados dos hifens na linha do cabeçalho.

### Markdown

```markdown
| Syntax      | Description | Test Texto |
| ----------- | ----------- | -----------
| Header      | Title       | Um pouco   |
| Paragraph   | Text        | De texto   |
```

### HTML

```html
<table>
	<thead>
		<tr class="header">
			<th style="text-align: left;">Sintax</th>
			<th style="text-align: center;">Descrição</th>
			<th style="text-align: right;">Teste Texto</th>
		</tr>
	</thead>
	<tbody>
		<tr class="odd">
			<td style="text-align: left;">Header</td>
			<td style="text-align: center;">Título</td>
			<th style="text-align: right;">Um pouco</th>
		</tr>
		<tr class="even">
			<td style="text-align: left;">Parágrafo</td>
			<td style="text-align: center;">Texto</td>
			<th style="text-align: right;">De texto</th>
		</tr>
	</tbody>
</table>
```

### Visualização

[Untitled](https://www.notion.so/63d10dd0afcd4abfaa52449c524cfcbe)

### Formatando texto em tabelas

Você pode formatar o texto em tabelas. Por exemplo, você pode adicionar links, código (palavras ou frases em crases (`) apenas, não blocos de código) e ênfase. 

Você não pode adicionar títulos, aspas, listas, regras horizontais, imagens ou tags HTML.

### Caracteres de escape de cachimbo nas tabelas

You can display a pipe (|) character in a table by using its HTML character code(&#124;)

## Blocos de código cercados

A sintaxe básica do Markdown permite que você crie blocos de codificação recuando linhas por quatro espaços ou uma guia. Se você achar isso inconveniente, tente usar blocos de código protegidos. Dependendo do seu processador ou editor Markdown, você usará três crases (```) ou três tils (~~~) nas linhas antes e depois do bloco de código. A melhor parte? Você não precisa recuar nenhuma linha!

### Markdown

```markdown
```
{
	"firstName": "John",
	"lastName": "Smith",
	"age": 25
}
```
```

### HTML

```html
<pre>
	<code>
	{
		&quot;firstName&quot;: &quot;John&quot;,
		&quot;lastName&quot;: &quot;Smith&quot;,
		&quot;age&quot;: 25
	}
	</code>
</pre>
```

### Visualização

```jsx
{
	"firstName": "John",
	"lastName": "Smith",
	"age": 25
}
```

### Destaque na sintax

Muitos processadores Markdown suportam realce de sintaxe para blocos de código protegidos. Este recurso permite adicionar realce de cor para qualquer idioma em que seu código foi escrito. Para adicionar realce de sintaxe, especifique um idioma próximo aos tiques anteriores antes do bloco de código protegido.

### Markdown

```markdown
```json
{
	"firstName": "John",
	"lastName": "Smith",
	"age": 25
}
```
```

### HTML

```html
<pre>
	<code class="language-json">
	{
		&quot;firstName&quot;: &quot;John&quot;,
		&quot;lastName&quot;: &quot;Smith&quot;,
		&quot;age&quot;: 25
	}
	</code>
</pre>
```

### Visualização

```json
{
	"firstName": "John",
	"lastName": "Smith",
	"age": 25
}
```

## Notas de rodapé

As notas de rodapé permitem adicionar notas e referências sem bagunçar o corpo do documento. Quando você cria uma nota de rodapé, um número sobrescrito com um link aparece onde você adicionou a referência da nota de rodapé. Os leitores podem clicar no link para acessar o conteúdo da nota de rodapé na parte inferior da página. 

Para criar uma referência de nota de rodapé, adicione um circunflexo e um identificador entre colchetes ([^ 1]). Os identificadores podem ser números ou palavras, mas não podem conter espaços ou tabulações. Os identificadores apenas correlacionam a referência da nota de rodapé com a própria nota de rodapé - na saída, as notas de rodapé são numeradas sequencialmente. 

Adicione a nota de rodapé usando outro acento circunflexo e número entre colchetes com dois pontos e texto ([^ 1]: Minha nota de rodapé.). Você não precisa colocar notas de rodapé no final do documento. Você pode colocá-los em qualquer lugar, exceto dentro de outros elementos como listas, blockquotes e tabelas.

### Markdown

```markdown
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

	Indent paragraphs to include them in the footnote.

	`{ my code }`

	Add as many paragraphs as you like.
```

### HTML

```html
<p>
	Here’s a simple footnote, <a href="#fn1"class="footnote-ref"id="fnref1"><sup>1</sup></a> and here’s a longer one. <a href="#fn2"class="footnote-ref"id="fnref2"><sup>2</sup></a>
</p>
<section class="footnotes">
	<hr/>
	<ol>
		<li id="fn1"><p>This is the first footnote.<a href="#fnref1" class="footnote-back">&#8617;&#xFE0E;</a></p></li>
		<li id="fn2">
			<p>Here’s one with multiple paragraphs and code.</p>
			<p>Indent paragraphs to include them in the footnote.</p>
			<p><code>{ my code }</code></p>
			<p>Add as many paragraphs as you like.<ahref="#fnref2"class="footnote-back">&#8617;&#xFE0E;</a></p>
		</li>
	</ol>
</section>
```

### Visualização

Here’s a simple footnote, $^1$ and here’s a longer one $^2$

## Heading IDs

Muitos processadores Markdown suportam IDs personalizados para cabeçalhos - alguns processadores Markdown os adicionam automaticamente. Adicionar IDs personalizados permite vincular diretamente aos títulos e modificá-los com CSS. Para adicionar um ID de título personalizado, coloque o ID personalizado entre chaves na mesma linha do título.

### Markdown

```markdown
### My Great Heading {#custom-id}
```

### HTML

```html
<h3 id="custom-id">My Great Heading</h3>
```

### Visualização

$^1$Esta é a primeira nota de rodapé.

$^2$Aqui está uma nota com vários parágrafos e código. Indique os parágrafos para incluí-los na nota de rodapé. 

`{Meu código}` 

Adicione quantos parágrafos quiser.

## Vinculando a IDs de título

Você pode vincular a cabeçalhos com IDs personalizados no arquivo criando um link padrão com um sinal numérico (#) seguido pelo ID do cabeçalho personalizado.

### Markdown

```markdown
[Heading IDs](#heading-ids)
```

### HTML

```html
<a href="#heading-ids">Heading IDs</a>
```

Outros sites podem vincular ao título adicionando o ID do título personalizado à URL completa da página da web (por exemplo, [IDs de título] ([https://www.eff.org/page#heading-ids](https://www.eff.org/page#heading-ids)))

## Listas de definição

Alguns processadores Markdown permitem que você crie listas de definições de termos e suas definições correspondentes. Para criar uma lista de definições, digite o termo na primeira linha. Na próxima linha, digite dois pontos seguidos por um espaço e a definição.

### Markdown

```markdown
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```

### HTML

```html
<dl>
	<dt>First Term</dt>
	<dd>This is the definition of the first term.</dd>
	<dt>Second Term</dt>
	<dd>This is one definition of the second term. </dd>
	<dd>This is another definition of the second term.</dd>
</dl>
```

### Visualização

**Primeiro termo**

This is the definition of the first term.

**Segundo termo**

This is one definition of the second term.

This is another definition of the second term.

## Palavra Tachada

Você pode "tachar" palavras colocando uma linha horizontal no centro de
eles. Este recurso permite que você indique que certas palavras são um erro sem intenção
para inclusão no documento. Para rasurar palavras, use dois símbolos de til () antes e depois das palavras.

### Markdown

```markdown
The world is ~~flat~~ round.
```

### HTML

```html
<p>The world is <del>flat</del> round.</p>
```

### Visualização

The world is ~~flat~~ round.

## Listas de Tasks

As listas de tarefas permitem que você crie uma lista de itens com caixas de seleção. Nos aplicativos Markdown que oferecem suporte a listas de tarefas, as caixas de seleção serão exibidas ao lado do conteúdo. Para criar uma lista de tarefas, adicione travessões (-) e colchetes com espaço ([]) na frente dos itens da lista de tarefas. Para selecionar uma caixa de seleção, adicione um x entre os colchetes ([x]).

### Markdown

```markdown
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

### HTML

```html
<p>The world is <del>flat</del> round.</p>
```

### Visualização

- [x]  Write the press release
- [ ]  Update the website
- [ ]  Contact the media

## Emoji

Existem duas maneiras de adicionar emoji a arquivos Markdown: copie e cole o emoji em seu texto formatado em Markdown ou digite códigos de atalho de emoji.

### Copiando e colando Emoji

Na maioria dos casos, você pode simplesmente copiar um emoji de uma fonte como Emojipedia e colá-lo em seu documento. Muitos aplicativos Markdown exibirão automaticamente o emoji no texto formatado em Markdown. Os arquivos HTML e PDF exportados de seu aplicativo Markdown devem exibir o emoji.

### Usando códigos Emoji

Alguns aplicativos Markdown permitem inserir emoji digitando códigos de atalho de emoji. Eles começam e terminam com dois pontos e incluem o nome de um emoji.

### Markdown

```markdown
Gone camping! :tent: Be back soon.

That is so funny! :joy:
```

## Vinculação automática de URL

Muitos processadores Markdown transformam URLs em links automaticamente. Isso significa que se você digitar [http://www.example.com](http://www.example.com/), seu processador Markdown o transformará automaticamente em um link, mesmo que você não tenha usado colchetes.

### Markdown

```markdown
http://example.com
```

### HTML

```html
<a href="http://example.com">http://example.com</a>
```

### Visualização

[http://example.com](http://example.com)

## Desabilitando a vinculação automática de URL

Se você não quiser que um URL seja vinculado automaticamente, você pode remover o link denotando o URL como um código com crases.

### Markdown

```markdown
`http://example.com`
```

### HTML

```html
<code>http://www.example.com</code>
```

### Visualização

http://example.com