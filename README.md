<h1 align="center">Documentação do Anúncios Koha Opac</h1>

<h2>
 Sobre
</h2>
Essa documentação foi feita para esclarecer ao administrador da biblioteca da forma mais simples de como criar e personalizar os anúncios do koha opac. Mas com detalhes de como se aprofundar na linguagem html e css.
<p>
OBS: Mesmo quem não entende nada de html ou css pode copiar o modelo pronto e estilizado de anúncio. Continue lendo essa documentação para mais detalhes
</p>

<br></br>
<h2>Sumario</h2>

- [Sobre o editor de texto](#sobre-o-editor-de-texto)
- [Uma breve introdução ao HTML](#uma-breve-introdução-ao-html)
- [Como estilizar os anúncios](#como-estilizar-os-anúncios)
- [Dicas de css](#dicas-de-css)
- [Sobre o Anúncio](#sobre-o-anúncio)
- [Anúncio Completo](#anúncio-completo)
- [Dúvidas](#dúvidas)

<!---->

 

# Sobre o editor de texto
<h2>Não pule essa etapa</h2>
Você pode querer testar como fica o anuncio antes de colocar no site koha opac, para saber mais sobre continue a leitura.
<br></br>
<h2>Para que preciso de um editor de texto?</h2>
Se você ja é um usuário experiente de computadores já deve saber sobre os editores de texto como word ou bloco de notas, eles servem para escrever alguns texto, porém não servem para editar o html e css, para fazer isso recomendo o uso do editor VScode, nele você consegue visualizar o documento html no navegador e é muito mais intuitivo, ele está disponivel em todas as plataformas, Windows, MacOS e Linux.
<br></br>
<h2>Sobre o VS Code</h2>
Ele é bem simples de usar e da pra personalizar como você quiser, mas esse não é o foco no momento, vou deixar o link para você instalar:
[Vs code](https://code.visualstudio.com/download)
<br></br>
<h3>Primeiros passos no vs code</h3>
primeiro crie um arquivo index.html, abra o arquivo usando o vs code. Caso você não saiba como usar o vs code, pesquise algum video no youtube de alguém que vai lhe ensinar a melhor forma de usar Vs code no seu sistema operacional, linux, windows ou macos.
Existe uma opção de que inicia um rascunho html para você não precisar se preocupar com isso, digite html:5, o proprio editor deve oferecer essa opção(html:5) clique para que o editor mostre o rascunho de html, caso esse rascunho não apareceu para você, cole o codigo abaixo no seu arquivo index.html:
```
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teste do anúncio</title>
</head>
<body>
     <!-- Escreva seu código html abaixo -->

     <!----------------->
</body>
</html>
```
Várias dessas tags html são tags de cofiguração e não há necessidade de explicar o que cada uma faz, elas são necessárias em todos os elementos html, agora que você colou o código acima, cole o código do fim da pagina dentro da tag body, [Código do Anúncio](#anúncio-completo).

<h3>Como visualizar meu anúncio no navegador?</h3>
Você precisa instalar uma extensão no Vs Code chamada "Live Server", é fácil de instalar, se você já está no seu arquivo html deve ter visto um menu lateral no lado esquerdo, existe uma opção com um icone com 4 quadrados no total, 3 juntos e 1 separado, caso não esteja encontrando esse icone passe o mouse em cima de cada icone que o próprio app vai mostrar o nome, escolha a opção "Extenções" e pesquise "Live Server" desenvolvida por "Ritwick Dey", clique na extensão para abrir a página, instale e verifique se está ativa.
Após instalar e ativar a extensão clique an opcção no canto inferior direito "go live" isso vai abrir uma pagina no seu navegador com o html do que jeito que vai ficar no site, demora alguns segundos então é necessário esperar.


<br></br>
# Uma breve introdução ao HTML
Essa sessão foi criada caso queira saber um pouco mais sobre html para modificar os anúncios do koha. Se você não pretende fazer modificações na estrutura do anúncio, e sim fazer modificações estéticas como cores e ordem dos elementos, pule essa sessão e vá para a parte de [Como estilizar os anuncios](#como-estilizar-os-anuncios)
<p>
O html é uma linguagem feita para criar paginas web.
Um elemento HTML é separado de outro texto em um documento por "tags", que consistem no nome do elemento entre "<" e ">". O nome de um elemento dentro de uma tag é insensível a maiúsREculas e minúsculas. Isto é, pode ser escrito em maiúsculas, minúsculas ou um mistura. Por exemplo, a tag 

`<title>` 
pode ser escrita como `<Title>`, `<TITLE>`.
</p>

```html
<html></html>
```

Exemplo de tag de abertura: 
```html
<html>
```

Exemplo de tag de fechamento:
```html
</html>
```

OBS: exisem tags que não possuem tag de fechamento, como nos exemplos baixo:
tag img para inserir imagens nas paginas web
```html
<img src="imagem_de_gato.jpg" alt="imagem de gato" >
```
a tag img é uma tag usada para imagens, caso queira saber mais sobre as tags html você pode acessar uma das duas documentações:<br></br>
[w3school](https://www.w3schools.com/html/default.asp)(Não possui versão em português. Recomendo acessar esse link)<br>
[mdn](https://developer.mozilla.org/pt-BR/docs/Web/HTML)(Possui versão em português. Não acho ruim porém eu prefiro o w3school)



<h2>Exemplo de tags interesante para você utilizar:</h2>
Essa sessão foi criada para dar exemplos de tags que você vai precisar para tarefas especificas porem não sabe a tag certa para essa tarefa.
<br></br>

<h2> Links </h2>
Se você quiser adicionar um link, utilize a tag ancora

```html
<a href="url do link, ex: http://youtube.com ou www.google.com">texto que vai aparecer</a>
```
Como fica visualmente:<br>
<a href="https://biblioteca-cfpm-semed.manaus.am.gov.br/">link</a>

mais informações:<br>
[tag a w3school](https://www.w3schools.com/tags/tag_a.asp)<br>
[tag a mdn](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/a)
<br></br>


<h2> Listas </h2>
Se você quiser fazer uma lista há duas maneiras de fazer, você pode fazer uma lista ordenada ou uma lista não ordenada. Como você pode ver no exemplo abaixo é preciso de 2 tipos diferentes de tags, a tag 

`<ol>` ou `ul` e a tag `<li>`<br>
Exemplo de lista ordenada:
```html
<ol>
    <li>Primeiro elemento</li>
    <li>Segundo elemento</li>
    <li>Terceiro elemento</li>
</ol>
```
Como fica visualmente:
<ol>
    <li>Primeiro elemento</li>
    <li>Segundo elemento</li>
    <li>Terceiro elemento</li>
</ol>
<br>
Mais informações sobre listas ordenadas:

[tag ol w3school](https://www.w3schools.com/tags/tag_ol.asp)<br>
[tag ol mdn](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/ol) 
<br></br>

A tag `<li>` é usada para os elementos de uma lista, você pode colocar quantas tags `<li>` você quiser, é de graça então pode usar à vontade :)<br>
Exemplo de lista não ordenada:
```html
<ul>
    <li>Primeiro elemento</li>
    <li>Segundo elemento</li>
    <li>Terceiro elemento</li>
</ul>
```
Como fica visualmente:
<ul>
    <li>Primeiro elemento</li>
    <li>Segundo elemento</li>
    <li>Terceiro elemento</li>
</ul>
<br>
Mais informações sobre listas não ordenadas:

[tag ul w3school](https://www.w3schools.com/tags/tag_ul.asp) <br>
[tag ul mdn](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/ul)
<br></br>


# Como estilizar os anúncios
Para se estilizar o html de uma página, se utiliza a linguagem css, através dela voce pode mudar cores, tamanhos e formato dos elementos html.
```css
seletor {
    propriedade: valor;
    color: red;
    background-color: black;
    margin: 1px 2px 3px 4px;
    padding: 4px 3px 2px 1px;
    width: 90%;
    font-size: 1.1em;
}
```

para se estilizar tags html você precisa selecionar a tag que você quer estilizar, substitua o "seletor" por o nome da tag html(`<a>, <input>, <div>, <button>, <div>`), nome da classe (`.Nome-do-elemento`) ou do id (`#Nome_do_id`).
<br></br>

Talvez você não tenha entendido o que é esse px, px é abreviação para pixel(s), ele é uma unidade de medida com valores fixos, que não vão e adaptar as mudanças em cada dispositivo então é bom ter um pouco de cuidado, porém existem outras unidades de medida fixas e relativas. Não irei colocar todas as unidades de medida, so aquelas mais relevantes, porém caso queira saber mais [clique no link](https://www.alura.com.br/artigos/guia-de-unidades-no-css)
<br></br>

<h2>Medidas Absolutas</h2>
Essas são as mais comuns que vemos no dia a dia. São medidas que não estão referenciadas a qualquer outra unidade, ou seja, não dependem de um valor de referência. São unidades de medidas definidas pela física, como o píxel, centímetro, metro, etc...

Essas medidas são fixas e não mudam de acordo com as especificações do dispositivo.
<br></br>

<h3>Pixel- px</h3>
O Pixel CSS - denotado no CSS pelo sufixo px - é uma unidade de comprimento que corresponde aproximadamente a largura ou altura de um ponto único que pode ser confortavelmente visto pelos olhos humanos sem esforço, mas é o menor possível.

```css
p {
    width: 500px;
}
```

<br>
<h3>Centímetro e Milímetro (cm / mm)</h3>
Nós brasileiros, que adotamos o sistema métrico, conhecemos bem essas duas medidas, que são bastante utilizadas no dia a dia. Apesar de bastante comuns, tanto centímetro e milímetro são pouco usadas no CSS. O uso dessa medida é esperado para folhas de estilo para impressões (medidas mais precisas), evitando que elas sejam aplicadas para exibições em tela.

```css
button {
    height: 10cm;
    padding-right: 10mm;
}
```
<br><br>
<h2>Medidas Relativas</h2>
Essas são as que normalmente não estamos habituados. Essas medidas são calculadas tendo como base uma outra unidade de medida definida, como por exemplo "em" e o "rem".

O uso delas é mais apropriado para que possamos fazer ajustes em diferentes dispositivos garantindo um layout consistente e fluido em diversas mídias.

Devido ao fato de que essas medidas são calculadas pelo browser baseando-se em outra unidade, elas tendem a ser bastante flexíveis. Ou seja, podemos ter resultados diferentes de acordo com o ambiente.
<br></br>

<h3>Em</h3>
Mas como funciona esse tal de em?Essa unidade muda para os elementos filhos de acordo com o tamanho da fonte (font-size) do elemento pai, então vamos lá. Digamos que temos o seguinte html, me permitindo a licença poética de utilizar a tag style:

```css
input {
    font-size: 2.5em; 
}
```
<br></br>
<h3>Rem</h3>
O REM vem como sucessor do EM e ambos compartilham a mesma lógica de funcionamento (font-size), porém a forma de implementação é diferente. Enquanto o em está diretamente relacionado ao tamanho da fonte do elemento pai, o rem está relacionado com o tamanho da fonte do elemento root (raiz), no caso, a tag.

O fato de que o rem se relaciona com o elemento raiz resolve aquele problema que tínhamos com diversas divs (elementos) aninhados, uma vez que não haverá essa "herança" de tamanhos, lembra?! Ou seja, não precisaremos ter dor de cabeça tendo que realizar cálculos, uma vez que nos baseamos na tag raiz.

```css
a {
    font-size: 3rem;
}
```
<br></br>
<h3>Porcentagem - %</h3>
utilizada quando falamos de layout responsivo e fluido, por isso, não poderia deixá-la passar.

A porcentagem permite que criemos módulos que sempre vão se readaptar para ocupar a quantidade especificada. Por exemplo, se definirmos um elemento tendo um tamanho de 50%, independente do dispositivo em questão, esse módulo sempre ocupará metade do espaço que lhe cabe (caso esteja dentro de algum outro elemento).
```css
div {
    width: 60%;
}
```

# Dicas de css

<h2>Margem - margin</h2>

Como ter um espaçamento entre dois items, no exemplo abaixo foi utilizado a tag div: 
```css
div {
    margin: 10px 20px 30px 40px;
}
```
Uma explicação sobre a propriedade "margin", como o nome sugere ele da uma margem de um elemento para outro, os valores estão em sentido horário começando 1º pela margem superior(10px), 2º margem direita(20px), 3º margem inferior(30px) e 4º margem esquerda (40px).
<br>
No exemplo acima foi utilizado 4 valores, um para cada lado, mas é possivel colocar 2 valores:

```css
div {
    margin: 10px 20px;
}
```
Nesse exemplo o valor de 10px é referente a margem vertical(margin superior e margem inferior) e o valor de 20px referente a margem horizontal(margem esquerda e margem direita).<br>
Também é possível colocar um único valor para todos os lados:
```css
div {
    margin: auto;
}

```
[w3school](https://www.w3schools.com/css/css_margin.asp) <br>
[mdn](https://developer.mozilla.org/pt-BR/docs/Web/CSS/margin)

<h2>Preenchimento - padding</h2>

A propriedade padding possui alguma semelhanças como margin: ambos são para dar espaçamento entre os elementos porem enquanto o margin é para espaçamento externo, o padding é para um elemento ou texto, exemplo, se tive um botão e você acha que o texto do botao está muito perto da borda, pode usar a propriedade padding, como no exemplo abaixo: 
```css
button {
    padding: 10px 20px 30px 40px;
}
```
Uma explicação sobre a propriedade "padding", como o nome sugere ele da uma preenchimento de um elemento para outro, os valores estão em sentido horário começando 1º pela margem superior(10px), 2º margem direita(20px), 3º margem inferior(30px) e 4º margem esquerda (40px).
<br>
No exemplo acima foi utilizado 4 valores, um para cada lado, mas é possivel colocar 2 valores:

```css
button {
    padding: 10px 20px;
}
```
Nesse exemplo o valor de 10px é referente a padding vertical(padding superior e padding inferior) e o valor de 20px referente a padding horizontal(padding esquerda e padding direita).<br>
Também é possível colocar um único valor para todos os lados:
```css
button {
    padding: auto;
}
```

[w3school](https://www.w3schools.com/css/css_padding.asp)
[mdn](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)

# Sobre o Anúncio
Nessa sessão vou falar de como funciona o anúncio, caso não queira entender sobre o anúncio, apenas vá para parte do [Anuncio completo](#anuncio-completo), se você veio nessa sessão porque quer fazer algumas modificações no anúncio, veio ao lugar certo.<br></br>

<h2>Como mudar a cor de fundo do anuncio</h2>
Se você alterar dessa forma todos os anúncios ficarão com  mesma cor, para deixar cada anúncio com uma cor diferente vá para para a parte de como deixar 2 anúncios com cores de fundo diferentes que está depois desse tópico.
Para o anúncio foi utilizado a tag section,

`<section></section>` com a class="Noticia" essa é a tag que contem todos os elementos do anúncio e possui essa estilização:
```css
    .Noticia {
          display: flex;
          flex-direction: row;
          background-color: #730d73;
          padding: 20px 10px;
          color: #fff;
          justify-content: space-evenly;
          margin: 6px;
        }
```

Se voce quiser mudar a cor do fundo do anúncio mude o valor da propriedade background-color, você pode colocar o nome da cor em inglês ou colocar em hexadecimal ou em rgb.
obs: se voce mudar a cor no css vai alterar a cor de todos os anúncios e evite colocar acentos e caracteres especiais

[Mais informações](https://celke.com.br/artigo/tabela-de-cores-html-nome-hexadecimal-rgb)

<h2>Como deixar 2 anúncios com cores de fundo diferente</h2>
Se você estiver colocando um segundo anúncio e quer deixar cada anúncio com uma cor de fundo diferente, procure a tag html e mude o valor da propriedade background-color, como exemplo abaixo. 
Se você pulou a parte de como estilizar um anuncio não deve ter entendido a propriedade background-color, ela serve para definir a cor de uma sessão, você pode color o nome das cores em inglês ou colocar o codigo da cor em hexadecimal ou rgb.

```html
<section class="Noticia" style="background-color: red;">
    <!-- resto do codigo html -->
</section>
```




# Anúncio Completo
so copie e cole o codigo abaixo na pagina de anúncio. Não esqueça de mudar o titulo, texto, data e imagem do anúncio.
```hml
<!-- Noticias -->
<!-- altere o valor da propriedade background-color -->
<section class="Noticia" style="background-color: blue;">
    <style>
        .Noticia {
          display: flex;
          flex-direction: row;
          background-color: #730d73; /* altere esse codigo #730d73 para o codigo de outra cor em heaxadecimal, não esqueça de colocar o # ele é necessário para pegar a cor, você tambem pode colocar em hexadecimal, em caso de duvida volte na sessão de estilização*/
          padding: 20px 10px;
          color: #fff;
          justify-content: space-evenly;
          margin: 6px;
        }

        .primeira-coluna {
          display: flex;
          flex-direction: column;
          width: 28%;
          justify-content: space-around;
          margin: 0 15px 0 5px;
        }

        .segunda-coluna {
          display: flex;
          flex-direction: column;
          justify-content: space-around;
          width: 38%;
          padding: 0 5%;
        }

        .terceira-coluna {
          display: flex;
          flex-direction: column;
          width: 34%;
        }

        .imagem-noticia {
          width: 95%;
          margin: auto;
        }

        .secao-instagram {
          display: flex;
          flex-direction: row;
          justify-content: center;
        }

        .logo-instagram {~
          text-align: center;
          font-size: 2em;
        }

        .span-quando {
          text-align: center;
          font-size: 1em;
          font-weight: bold;
        }

        .span-onde {
          text-align: center;
          font-size: 1em;
          font-weight: bold;
        }

        .paragrafo-noticia {
          text-align: center;
        }

        .id-instagram{
          font-size: 1.2em;
          margin-left: 2px;
          color: #fff;
        }

        .div-informacoes {
          display: flex;
          flex-direction: column;
        }

        @media screen and (max-width: 800px) {
            .Noticia {
                flex-direction: column;
            }

            .secao-instagram {
                display: none;
            }

            .primeira-coluna {
                width: 100%;
                margin-bottom: 10px ;
            }

            .segunda-coluna {
                width: 100%;
            }

            .terceira-coluna {
                width: 100%;
                justify-content: center;
                margin-top: 15px;
            }

            .titulo-noticia {
                font-size: 1.5em;
            }

            .paragrafo-noticia {
                text-align: center;
            }
        }
      </style>
    <div class="primeira-coluna" style="order: 1;">
        <!-- Altere aqui o nome do Titulo do anúncio-->
        <h2 class="titulo-noticia">
            Mude o nome da escola
        </h2>
        <div class="secao-instagram">
            <img src="https://inovape-comunicacoes.github.io/projeto-koha/imagens//icons8-instagram-256.png" alt="logo instagram" class="logo-instagram" 
            /> 
            <!-- Altere aqui o link e o texto do link para instagram-->
            <a 
                class="id-instagram" 
                href="https://www.instagram.com/semedmanaus/"
            > 
                @Semed_Oficial 
            </a>
        </div>
    </div>
    <div class="segunda-coluna" style="order: 2;">
    <!-- Altere aqui o texto do anúncio -->
        <p class="paragrafo-noticia">        
                "Ler &eacute;     legal a qualquer hora" foi o lema usado na produ&ccedil;&atilde;o teatral e no incentivo na forma&ccedil;&atilde;o dos leitores. As escolheram o livro e produziram a pe&ccedil;a com orienta&ccedil;&atilde;o do biblioec&aacute;rio e professores. Agora est&atilde;o convidado a comunidade para participarem da apresenta&ccedil;&atilde;o.
        </p>
        <div class="div-informacoes">
            <!-- Altere aqui a data do anúncio -->
            <span class="span-quando"> 
                Quando: 23/06/2023 
            </span> 
            <!-- Altere aqui o local  -->
            <span class="span-onde">
                Onde: Quadra da escola             
            </span>
        </div>
    </div>
    <div class="terceira-coluna" style="order: 3;">
        <!-- Altere aqui a imagem do anúncio -->
        <img 
            src="https://www.canoas.rs.gov.br/ wp-content/uploads/2019/08/Pablo-Reis-30.jpg" alt="professora dando uma palestra" class="imagem-noticia" />
    </div>
</section>
<!-- Fim das Noticias-->
```


# Dúvidas
<h2>Alguns casos de erro</h2>
Caso você tenha seguido todo o passo a passo e mesmo assim tenha acontecido um erro é bom verificar
se todos os sinais foram colocados, exemplo "<", ">", "{", "}". 
