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
