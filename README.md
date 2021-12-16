# AngularJsTextEditor
Melhorias que foram feitas nesse projeto.

1. Encapsulado o rangy em um módulo angularjs
   - Essa mexida tem o intuito de evitar problemas caso se utilize o webpack como bundle
2. Ajustado UI do componente
3. Ajustado angularjstexteditorSanitize para ser compátivel com versões mais novas do angularJs
4. Melhorias de estilo
5. Ajustado build para ser feito utilizando gulp
6. Removido alguma ferramentas que não estavam sendo utilizadas

# Como deve ser utilizado?
Para que o componente funcione é necessário ter as importações na seguinte ordem:

```html
  <script src="../dist/angularjstexteditorSanitize.min.js"></script>
  <script src="../dist/angularjstexteditorRangy.min.js"></script>
  <script src="../dist/angularjstexteditorSetup.min.js"></script>
  <script src="../dist/angularjstexteditor.min.js"></script>
```
### Para não ter problemas com algumas tags ou estilos se perdendo, o componente deve estar conforme abaixo

```html
     <angularjstexteditor ta-keep-styles="true" ng-model="vm.meuTextoPersonalizado" ta-unsafe-sanitizer="true">
      </angularjstexteditor>
```
=======
## angularjstexteditor v1.2.5
===========

## Notas da versão
```html
   <ul>
      <li>Ajustes no tratamento de links do youtube ao inserir vídeos</li>
   </ul>
```

## Requisitos

1. `AngularJS` ≥ `1.3.x` Caso utilize a versão acima de 1.6.* terá problemas com lowercase
2. `Rangy` ≥ `1.3.x`,
3. `Font-Awesome` ≥ `4.x` Preferência a mais recente
1. `Bootstrap` ≥ `3.x` Preferência a mais recente

## Aviso

Caso utilize o angularjstexteditor em uma versão acima do 1.6.8 terá problemas com angular lowercase, pois a sintaxe muda de uma versão para outra. 


**Via Bower:**

Rode `bower install angularjstexteditor` Por linha de comando, lembre-se de especificar a versão que vai utilizar.
Inclua as tags similar ao código abaixo:

```html
<link rel='stylesheet' href='your_path/angularjstexteditor/dist/angularjstexteditor.css'>
<script src='your_path/angularjstexteditor/dist/angularjstexteditor-rangy.min.js'></script>
<script src='your_path/angularjstexteditor/dist/angularjstexteditor-sanitize.min.js'></script>
<script src='your_path/angularjstexteditor/dist/angularjstexteditor.min.js'></script>
```


## FAQ

Caso tenha problemas com os estilos do tamanho da fonte, color e background-color, utlize a tag 'ta-keep-styles="true"'.

```html
   <angularjstexteditor ta-keep-styles="true"  ng-model="vm.yourModel"></angularjstexteditor>
```

Caso tenha problemas com inserção de vídeos utilize a tag 'ta-unsafe-sanitizer="true"'

```html
    <angularjstexteditor ta-keep-styles="true" ta-unsafe-sanitizer="true" ng-model="vm.yourModel"></angularjstexteditor>
```

## Licença
Este projeto é licenciado por [MIT license](http://opensource.org/licenses/MIT).

## Contribuidores

<a href="https://github.com/EbenauDev" target="_blank">João Tiago</a>
