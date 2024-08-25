# HTML5 E CSS3

## HTML

### Estrutura básica de um documento HTML:

```
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset=""UTF-8>
    <title>Nome do documento</title>
  </head>

  <body>

  </body>

</html>
```

`h1` -> Cria um título <br>
`hr` -> Cria uma linha horizontal <br>
`p` -> Cria um parágrafo <br>
`br` -> Quebra um texto <br>
`&lt;` -> Cria um < <br>
`&gt;` -> Cria um > <br>

### Gimp
- É usado para edição de imagens para sites de forma mais simplificada
- Imagem > Redimensionar imagem (Muda o tamanho da imagem proporcionalmente)
- O ideal é sempre guardar as imagens full, para uma futura necessidade
- Quando uma imagem é alterada no CSS, ela ainda possui o mesmo tamanho, ou seja, ocupa mais espaço

### Adição de imagens
`<img src="nome-da-imagem.png" alt="Descrição da imagem">`

### Favicon
- O melhor formato para se usar em um favicon é o .ico
- iconarchive é um site que possui algumas logos genéricas para sites simples
- favicon.cc é um site para criação de ícones manualmente
- favicon.io cria um .ico com base em um texto, um png ou um emoji
- No html, o favicon é adicionado dentro do `<head>`
- `link:favicon` + enter, puxa toda a estrutura no Vscode
- Estrutura completa: `link real="shortcut icon" href="favicon.ico" type="image/x-icon">`

### Hierarquia de Títulos
- Títulos possuem 6 níveis de hierarquia: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`. Sendo `<h2>` um sub-assunto de `<h1>` e assim por diante


### Semântica dentro do HTML
- A maior adição do HTML5 foi a semântica, ou seja, a adição de significado à um conjunto de palavras.
- Por exemplo: É um lugar lindo de se morar, ficando na `<adress>`Rua dos Bobos, 0`</adress>`
- Foi adicionado um sentido "adress" à um endereço. Possibilitando que, por exemplo, um navegador de celular possa sugerir como um endereço no gps.
- O intuito da W3C, que normatiza o html, é deixar as tags cada vez mais semânticas, deixando os estilos apenas para o CSS.
- Existem tags que estão se tornando obsoletas, como `<font>` e `<center>` e otras que já foram excluídas, como `<blink>`.
- A própria W3C sugere usar `<strong>` para textos em negrito no lugar de `<b>`, pois descreve um texto forte e não apenas um negrito.
- Algumas tags utilizadas:
    - `<strong>` -> negrito
    - `<em>` -> Itálico
    - `<mark` -> Destacado
    - `<del>` -> Riscado
    - `<ins>` -> Sublinhado
    - `<sub>` -> Sobrescito
    - `<sup>` -> Subscrito
    - `<code>` -> Para Códigos
    - `<pre><code>` -> Também para códigos, mas com tabulações corretas
    - `<q>`-> Para citações dentro de um texto
    - `<blockquote>` -> Para um parágrafo inteiro de cirações
    - Pode-se usar o parâmetro `cite` para direcionar para o texto original:<br>
      ```
      <blockquote cite="https://www.siteoriginal.com/citacao">
        Na minha terra tem palmeiras onde canta o sabiá...
      </blockquote>
      ```
    - `<abbr>` -> Para abreviações<br>
      ```
      <p>Eu estou estudando <abbr title="Hyper Text Markup Language">HTML</abbr> para criar sites.</p>
      ```

### Listas
- Lista ordenada:
    - Para criar uma lista ordenada, usa-se a tag `<ol>` para delimitação e `<li>` para cada item.
      ```
      <ol type="tipo" start="primeiro item">
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
        <li>Item 4</li>
      </ol>
      ```
    - Tipos de Lista Ordenada:
      - 1 - Valor padrão, com lista numerada
      - A - Lista separada por letras maiúsculas
      - a - Lista separada por letras minúsculas
      - I -> Algarismos romanos maiúsculos
      - i -> Algarismos romanos minúsculos

- Lista não ordenada
  - Para criar uma lista não ordenada, usa-se a tag `<ul>` para delimitação e `<li>` para cada item.
    ```
    <ul type="tipo">
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
      <li>Item 4</li>
    </ul>
    ```
  - Tipos de lista não ordenada:
      - disc -> padrão, bola preta totalmente pintada
      - circle -> bola com borda preta sem preenchimento
      - square -> quadrado totalmente pintado
   
### Links
- Para criar um link, é criado uma âncora `<a>` com o atributo `href` com o link desejado.
  ```
  <a href="www.link.com">Acesse meu Link</a>
  ```
- Pode-se usar o atributo `hreflang` para específicar o idioma do site presente no link
- Pode-se usar o atributo `target` para especificar se o link vai ser aberto na mesma ou em outra janela.
  ```
  <a href="www.link.com" target="_self">
    Continuar navegando no site
  </a>
  ```
  <br>
  
  ```
  <a href="www.link.com" target="_blank">
    Abrir site em outra janela
  </a>
  ```

- Para downloads, basta utilizar o atributo `download` com o nome do arquivo a ser baixado.
  ```
  <a href="livro.pdf" download="livro.pdf" type="application/pdf">
    Baixe arqui o PDF do meu livro
  </a>
  ```
  - media types mais comuns:<br>
    ‣ application/zip<br>
    ‣ text/html<br>
    ‣ text/css<br>
    ‣ text/javascript<br>
    ‣ video/mp4<br>
    ‣ video/H264<br>
    ‣ video/JPEG<br>
    ‣ audio/aac<br>
    ‣ audio/mpeg<br>
    ‣ font/ttf<br>
    ‣ image/jpeg<br>
    ‣ image/png<br>

### Áudio
`<audio src="musica.mp3" controls autoplay></audio>`

### Vídeo
`<video src="meu-video.mp4" width="500" poster"thumbnail.png" controls></video>`

## CSS

### Psicologia das cores
- Cores são mais importantes do que parecem
- A harmonia visual de um site pode prender 90% mais pessoas
- Azul: É muito usado em empresas de tecnologia, tem ligação com competência, calma, segurança e profissionalismo. É a cor com menor taxa de rejeição.
- Vermelho: Associado para entretenimento e comida.
- Amarelo: Remete a felicidade, também muito usado por sites de comida.
- Verde: Tem a ver com ecologia, natureza, dinheiro.
- Rosa: Muito usado para produtos femininos, como cosméticos, passa um tom mais delicado
- Marrom: Pode trazer uma ideia de luxo ou de robustês

### Harmonia de cores
- Círculo cromático: Possui milhões de cores, é utilizado para harmonizar as cores.
    - Cores primárias: Amarelo, Vermelho, Azul
    - Cores secundárias: Laranja, vermelho e verde
    - Cores terciárias: A mistura de cores primárias com secundárias

![image](https://github.com/user-attachments/assets/5dccdf57-5a3e-4c42-abd2-48db1b77776e)

- Temperatura, podem ser divididas em quentes e frias:
![image](https://github.com/user-attachments/assets/ea47ef15-2597-409e-bc7f-ace5739c5c3f)

- Cores complementares: São as que apresentam maior contraste, ficam do lado posto do círculo cromático:
![image](https://github.com/user-attachments/assets/0aa24d78-60c5-4e22-b325-1f056ac440fd)

- Cores análogas: São as cores vizinhas entre si
![image](https://github.com/user-attachments/assets/5e001780-4487-4553-bf03-17c1acb7f395)


- Adobe color: Cria paletas e extrai paletas de logo
- Paletton: Aplica em um exemplo de site
- Coolors: Dá sugetões aleatórias

### Gradiente no CSS (background)
`background-image: linear-gradient(to right, white, blue);`



