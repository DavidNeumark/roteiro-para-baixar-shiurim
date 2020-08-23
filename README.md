Nosso script comeca na pagina aonde esta a lista completa dos shiurim do rabino, neste [link](http://beinenu.com/faceted_search/results/field_rabbi4lesson%3A43971)
Podemos comecar a busca selecionando חומש בראשית na lista de shiurim, o que nos leva a uma pag. com uma lista de todos os shiurim do livro בראשית.
Obs.: Obviamente, repetir todo o processo nos outros 4 livros (שמות, ויקרא...).
[link para a lista de shiurim no livro Bereshit selecionado](http://beinenu.com/faceted_search/results/taxonomy%3A47499%20field_rabbi4lesson%3A43971)
A lista e bastante longa e foi divida em 7 paginas.

Antes de entrar no primeiro shiur e' importante guardar na memoria o nome da parasha e o ano que estao ressaltadas na pag. e entao acessar o video: [link](http://beinenu.com/lessons/%D7%A4%D7%A8%D7%A9%D7%AA-%D7%91%D7%A8%D7%90%D7%A9%D7%99%D7%AA-17)

No final das contas nas queremos "personalizar" e rodar o seguinte comando para cada shiur:
curl -H "Referer: http://vod.wgnmedia.com/VOD/vod.php\?ID\=74645\&CS\=26" http://vod.wgnmedia.com/VOD/LIB.MP4/v74645.mp4 --output bereshit-5779.mp4

F12 > Network > clicar play no video > localizar o arquivo mp4 e copiar o curl >
  '''
  curl 'http://vod.wgnmedia.com/VOD/LIB.MP4/v74645.mp4' \
    -H 'Referer: http://vod.wgnmedia.com/VOD/vod.php?ID=74645&CS=26' \
    -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/84.0.4147.125 Safari/537.36' \
    -H 'Range: bytes=1966080-' \
    --compressed \
    --insecure
  '''
![lista-completa.png](lista-completa.png)

https://stackoverflow.com/questions/36433755/ghematria-in-python-hebrew-letters-to-numbers-and-sum
