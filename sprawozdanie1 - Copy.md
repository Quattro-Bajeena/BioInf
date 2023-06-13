# Sekwencjonowanie łańcuchów DNA z błędami negatywnymi i pozytywnymi
Autor: *Mateusz Oleszek, nr. 144608*

## Parametry Uruchamiania algorytmu

Wielkość populacji = 100
Procent wyboru najlepszych z populacji = 0.2
Prawdopodobieństwo krzyżówki = 0.5
Prawdopodbieństwo mutacji = 0.3
Iteracje = 10

## Wyniki

Niestety po przeprowadzeniu wielu prób z różnymi wartościami wielkości populacji, iteracjami i parametrami odpowiadającymi za prawdopodobieństwo zajścia krzyżówki i  mutacji dla żadnej instancji nie udało się skonstruować pełnej ścieżki po grafie, czyli sekwencji z wykorzystaniem wszystkich oligonukleotydów.

## Obserwacje

Jak można się spodziewać, im więcej oligonukleotydów w instancji tym dłużej się ona wykonywała.

<img src="C:\Users\motme\AppData\Roaming\Typora\typora-user-images\image-20230613234150300.png" alt="image-20230613234150300" style="zoom:50%;" />

Zauważyłem też, że przy jakość rozwiązania różni się dla różnych typów instancji. Dla tych błędami pozytywnymi losowymi udało się znaleźć najlepsze rozwiązania, a te z negatywnymi losowymi były najtrudniejsze.

<img src="C:\Users\motme\AppData\Roaming\Typora\typora-user-images\image-20230613233847710.png" alt="image-20230613233847710" style="zoom:50%;" />

## Tabela z wynikami
|Filename|Max no. of nodes|Max Sequence length|Instance type|Time|No. of nodes|Sequence length|Percent of nodes used|
|:----|:----|:----|:----|:----|:----|:----|:----|
|10.500-100|500|509|negatywnymi losowymi|29|391|508|0.78|
|10.500-200|500|509|negatywnymi losowymi|16|284|509|0.57|
|18.200-40|200|209|negatywnymi losowymi|5|155|225|0.78|
|18.200-80|200|209|negatywnymi losowymi|2|107|209|0.54|
|20.300-120|300|309|negatywnymi losowymi|6|156|308|0.52|
|20.300-60|300|309|negatywnymi losowymi|10|225|309|0.75|
|25.500-100|500|509|negatywnymi losowymi|31|385|509|0.77|
|25.500-200|500|509|negatywnymi losowymi|17|286|506|0.57|
|35.200-40|200|209|negatywnymi losowymi|5|155|209|0.78|
|35.200-80|200|209|negatywnymi losowymi|3|116|209|0.58|
|53.500-100|500|509|negatywnymi losowymi|28|375|508|0.75|
|53.500-200|500|509|negatywnymi losowymi|17|281|520|0.56|
|55.300-120|300|309|negatywnymi losowymi|7|174|305|0.58|
|55.300-60|300|309|negatywnymi losowymi|10|219|309|0.73|
|55.400-160|400|409|negatywnymi losowymi|10|212|409|0.53|
|55.400-80|400|409|negatywnymi losowymi|18|291|403|0.73|
|58.300-120|300|309|negatywnymi losowymi|6|172|326|0.57|
|58.300-60|300|309|negatywnymi losowymi|11|232|309|0.77|
|62.400-160|400|409|negatywnymi losowymi|11|226|409|0.57|
|62.400-80|400|409|negatywnymi losowymi|19|307|409|0.77|
|68.400-160|400|409|negatywnymi losowymi|10|221|409|0.55|
|68.400-80|400|409|negatywnymi losowymi|19|297|424|0.74|
|9.200-40|200|209|negatywnymi losowymi|5|151|208|0.76|
|9.200-80|200|209|negatywnymi losowymi|2|114|208|0.57|
|113.500-8|500|509|negatywnymi wynikającymi z powtórzeń|46|480|509|0.96|
|144.500-12|500|509|negatywnymi wynikającymi z powtórzeń|49|474|508|0.95|
|28.500-18|500|509|negatywnymi wynikającymi z powtórzeń|45|455|509|0.91|
|34.500-32|500|509|negatywnymi wynikającymi z powtórzeń|43|464|504|0.93|
|59.500-2|500|509|negatywnymi wynikającymi z powtórzeń|43|439|509|0.88|
|10.500+200|500|509|pozytywnymi losowymi|50|476|509|0.95|
|18.200+80|200|209|pozytywnymi losowymi|6|173|209|0.87|
|20.300+120|300|309|pozytywnymi losowymi|15|268|309|0.89|
|25.500+200|500|509|pozytywnymi losowymi|50|475|509|0.95|
|35.200+80|200|209|pozytywnymi losowymi|7|184|209|0.92|
|53.500+200|500|509|pozytywnymi losowymi|47|473|509|0.95|
|55.300+120|300|309|pozytywnymi losowymi|17|295|309|0.98|
|55.400+160|400|409|pozytywnymi losowymi|31|371|409|0.93|
|58.300+120|300|309|pozytywnymi losowymi|17|282|307|0.94|
|62.400+160|400|409|pozytywnymi losowymi|30|383|408|0.96|
|68.400+160|400|409|pozytywnymi losowymi|30|370|409|0.93|
|9.200+80|200|209|pozytywnymi losowymi|7|197|206|0.99|
|10.500+50|500|509|pozytywnymi, przekłamania na końcach oligonukleotydów|37|434|506|0.87|
|18.200+20|200|209|pozytywnymi, przekłamania na końcach oligonukleotydów|5|170|209|0.85|
|20.300+30|300|309|pozytywnymi, przekłamania na końcach oligonukleotydów|12|250|309|0.83|
|25.500+50|500|509|pozytywnymi, przekłamania na końcach oligonukleotydów|35|426|509|0.85|
|35.200+20|200|209|pozytywnymi, przekłamania na końcach oligonukleotydów|6|164|209|0.82|
|53.500+50|500|509|pozytywnymi, przekłamania na końcach oligonukleotydów|36|420|509|0.84|
|55.300+30|300|309|pozytywnymi, przekłamania na końcach oligonukleotydów|13|254|309|0.85|
|55.400+40|400|409|pozytywnymi, przekłamania na końcach oligonukleotydów|24|330|409|0.83|
|58.300+30|300|309|pozytywnymi, przekłamania na końcach oligonukleotydów|13|269|309|0.90|
|62.400+40|400|409|pozytywnymi, przekłamania na końcach oligonukleotydów|24|345|408|0.86|
|68.400+40|400|409|pozytywnymi, przekłamania na końcach oligonukleotydów|22|330|409|0.83|
|9.200+20|200|209|pozytywnymi, przekłamania na końcach oligonukleotydów|6|184|209|0.92|

