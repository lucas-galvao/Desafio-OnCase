# Desafio-OnCase

O código começa importando as bibliotecas necessárias para executá-lo.

Após importar as bibliotecas são obtidos publicações de 4 portais sobre tecnologia, são eles:
	- https://www.tecmundo.com.br/
	- https://www.techtudo.com.br/
	- https://olhardigital.com.br/
	- https://canaltech.com.br/

Foram extraido de cada site entre as 5 e 15 primeiras páginas com as postagens mais recentes, a quantidade de página foi determinada de acordo com a quantidade de postagens que cada site dispõem por página.

Dos sites foram extraidos os seguintes dados:
	- Título da matéria
	- Conteúdo da matéria
	- Data de publicação
	- Hora de publicação
	- Autor da matéria
	- Tags associadas à matéria

Tentei retirar a quantidade de comentários e compartilhamentos que cada publicação teve, porém só consegui esses dados para o site Tecmundo.

O conjunto de dados de cada site foram armazenados em dataframes para cada um dos portais e depois agrupados em um dataframe único.

Para a análise dos dados decidi utilizar gráficos de barras.

A primeira análise foi das tags utilizadas, para isso foram criados dicionários contendo a tag e a quantidade de vezes em que essa foi utilizada. Depois foram gerados os gráficos utilizando as duas variáveis. O primeiro foi analisando o total para todos os 4 portais, depois foram gerados gráficos para cada um dos sites.

Junto com os gráficos também foi analisado a redundância do uso tags. Em alguns sites foi encontrado que muitas tags são usadas em conjunto e em alguns casos temos tags contidas em outras. Quando a interseção entre o conjunto representa uma parcela significativa das observações foi desconsiderados os resultados da tag mais específica.


A segunda análise focou na quantidade de postagens por dia de cada site. Para encontrar esse valor foi considerado o dia 03 de outubro completo. Foi encontrado que os sites se dividem em 2 grupos: 
	- Canaltech e Olhar Digital: acima de 50 postagens por dia
	- Tecmundo e Techtudo: Entre 30 e 35 postagens por dia

A terceira análise foi feita sobre a repercusão das postagens do site Tecmundo. Essa análise foi feita apenas no site Tecmundo pois foi o único que obtive os dados de compartilhamentos e comentários.

Para análise foi observado quais tags possuem maior quantidade de comentários e compartilhamentos. Foram utilizadas 4 medidas:
	- Quantidade de comentários absoluta
	- Quantidade de compartilhamentos absoluta
	- Quantidade de comentários médio por postagem
	- Quantidade de compartilhamentos médio por postagem
