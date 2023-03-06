# manipulando-arquivos-de-texto
Programa que executa um arquivo de texto com nomes e preços de produtos e manipula os dados mostrando a média de preço e o nome dos produtos que estão abaixo dessa média.

-Class Product-

A classe Product contém as propriedades NAME e PRICE, e um construtor que utilizo no Programa Principal.

![sist1](https://user-images.githubusercontent.com/106346422/223174768-90c2ebc5-9001-4a59-b375-56d932babc09.png)


-Class Program-

No programa principal eu entro com o caminho do arquivo que será aberto e lido e depois crio uma lista. Como é um arquivo do tipo CSV, eu criei um vetor de strings usando o método .SPLIT(','), nesse caso o método separa as posições do meu vetor de acordo com a vírgula.
Feito isso, eu uso o STREAMREADER para abrir e e ler o aquivo e um WHILE para ele efetuar a leitura do aquivo até o final. Após, eu adiciono as variáveis já divididas do vetor dentro da liste criada anteriormente usando o construtor feito na classe PRODUCT.

Depois eu crio uma variável (VAR AVG) que recebe a média de preço dos produtos a partir de uma expressão Lambda com uma função que calcula a média e imprimo na tela essa valor.

Agora eu preciso especificar os nomes dos produtos que tem o preço abaixo dessa média. Crio outra váriavel que recebe uma expressão Lambda com métodos que fazem com que o resultado seja uma lista em ordem decrescente dos nomes desses produtos abaixo da média.
Por fim, eu faço um laço FOREACH passando por dentro da lista e pegando todos nomes que vieram do método anterior e imprimo na tela.

![sist2](https://user-images.githubusercontent.com/106346422/223182848-b8d1b537-44ec-44ab-9fdb-54264794e79f.png)

