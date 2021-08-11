# Curso CSS3
> Este repositório contém o que eu estou aprendendo no curso de CSS3. Nele possui exemplos de comandos e também projetos para praticá-los.


## Introdução
O CSS3 é a terceira versão do CSS (Folha de Estilo em Cascata), que tem como função definir estilos para páginas web. Com ele, podemso customizar elementos HTML, como adicionar imagens, backgrounds, fontes, cores, entre muitos outros.

## Conteúdo
No CSS3 podemos realizar as formatações de três maneiras:
* External Style Sheet
* Internal Style Sheet
* Inline Style 

No Inline Style, aplicamos a formatação diretamente no elemento, na Internal Style Sheet, colocamos o estilo dentro do código, enquanto no External Style Sheet, criamos um arquivo só para as formatações(recomendado).

### Inline Style

```
<h1> Estilo CSS (Cascading Style Sheets)</h1>
<p style="color:orange">
    Bacon ipsum dolor amet spare ribs ham biltong shankle 
    jerky, rump meatloaf salami.
</p>
<p style="color: green"> 
    Bacon ipsum dolor amet spare ribs ham biltong shankle 
    jerky, rump meatloaf salami.
</p>
```
#### Resultado:
<img src="Prints Exemplos\inline_exemplo.png">


### Seletores

Podemos utilizar seletores para a estilização, a estrutura deles é formada pela tag HTML que desejamos formatar e as propriedades que desejamos estilizar.

Exemplo(Internal Style Sheet):

```
<style type="text/css">
    p {
        color: red;
    }
    h1 {
        color: blue;
    }
</style>
```
#### Resultado:
<img src="Prints Exemplos\seletores_exemplo.png">

### Classes e IDs
Um Id é um identificador, utilizamos para definir a estilização de um único intem. Por outro lado, temos as Classes, que podem ser usadas para estilizar vários elementos. 

Exemplos:
```
<style type="text/css">
    /*Classe para definir cor azul*/
    .azul {
        color: blue;
    }
    /*Id principal*/
    #principal {
        background: orange;
    }
</style>
```
```
<body id="principal">
    <h1> Estilo CSS (Cascading Style Sheets)</h1>
    <p class="azul">
        Bacon ipsum dolor amet spare ribs ham biltong shankle 
        jerky, rump meatloaf salami.
    </p>
    <p class="azul"> 
        Bacon ipsum dolor amet spare ribs ham biltong shankle 
        jerky, rump meatloaf salami.
    </p>
</body>
```
#### Resultado:
<img src="Prints Exemplos\classes_ids_exemplo.png">

### Div e Span
A Div é uma divisão que pode ser utilizada para agrupar elementos. Por padrão, ela é um elemento do tipo block, ou seja, ocupa toda a largura da tela.
Já o Span, agrupa os elementos linha por linha, não ocupando a tela toda.

```
<style type="text/css">
    #conteudo {
        background: red;
    }
    #rodape {
        background: yellow;
    }
    .produto {
        background: gray;
        /*Margem*/
        margin: 10px; 
    }
    .azul {
        background: blue;
    }
</style>

```
```
<div id="conteudo">
    <div class="produto">
        Produto 1
    </div>
    <div class="produto">
        Produto 2
    </div>
    <div class="produto">
        Produto 3
    </div>
</div>
<div id="rodape">
    Todos os <span class="azul">direitos</span> reservados
</div>
```

#### Resultado:
<img src="Prints Exemplos\div_span_exemplo.png">

### Bordas
Como o nome ja diz, podemos utilizar bordas nas tags html. Para criar uma borda, definimos sua espessura, seu estilo e a cor. Podemos fazer de duas maneiras: <br>
Definindo suas característica em uma linha só:
```
border: 5px solid red;
```
Definindo cada característica separadamente:
```
border-color: blue yellow green orange;
border-width: 15px;
border-style: outset;
```
Definir as características da borda separadamente, nos dá a vantagem de definir cada lado da borda.<br>
#### Exemplo:
<img src="Prints Exemplos\bordas_exemplo.png">
Para mais exemplos de estilos de bordas, podemos acessar esse <a href="https://www.w3schools.com/css/css_border.asp">link</a>.

### Fontes e Cores
Podemos definir as cores no css de várias maneiras, para as cores mais simples, podemos simplismente escrever o nome delas.
<br>
Exemplo:
```
color : red;
```
Para cores mais complexas, podemos utilizar seu código no formato hexadecimal, como no exemplo a seguir:
```
color: #AB11CD;
```
Também, podemos utilizar seu código rgb da seguinte maneira:
```
color: rgb(255, 0, 255);
```
#### Resultado: 
<img src="Prints Exemplos\cores_exemplo.png">

Podemos definir, também, as fontes para os nossos textos, definindo o tamanho e também a família da fonte. Ao escolher a família da fonte, estamos definindo uma prioridade, pois se o usuário não possuir aquela fonte, ele passa para a próxima até uma fonte genérica.

```
.formatacao {
    font-size: 20px;
    font-family: "Times New Roman", Times, serif;
}
```

#### Resultado:
<img src="Prints Exemplos\fontes_exemplo.png">

### Tamanho de textos
Podemos definir o tamanho dos nossos textos, utilizando essas 3 formas. Podemos definir por pixels, que é uma forma fixa.
```
font-size: 60px;
```
De maneira relativa, podemos utilizar % ou 'em' para definir o tamanho do texto de acordo com o container pai.
```
font-size: 2em;
font-size: 50%;
```
Ao definirmos o tamanho do conteiner pai com 60px, uma fonte de tamanho 2em seria o dobro, ou seja, 120px, enquanto 50% seria a metade, que é 30px.

#### Resultado:
<img src="Prints Exemplos\tamanho_textos_exemplo.png">

### Estilos de textos
Para definir os estilos dos textos, podemos fazer de diversas maneiras, para escrever um texto em negrito, podemos escrever 'bold' ou um número de 100 a 900 para definir o nível, por exemplo:
```
font-weight: 900;
```
Para escrever um texto em itálico, podemos utilizar o seguinte código:
```
font-style: italic;
```
Para colocar linhas no textos, podemos utilizar destas 3 formas:
```
text-decoration: underline;
text-decoration: overline;
text-decoration: line-through;
```
Além disso, podemos realizar essas formatações de uma só vez, podendo agrupar essas características em uma linha.
```
font: bold 40px 'Times New Roman', Times, serif;
```
#### Resultado
<img src="Prints Exemplos\estilo_textos_exemplo.png">
