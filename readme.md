234844 / 13 = 18064 r. 12

Data taken from https://github.com/ogirardot/meta-deps/blob/master/mvn-deps.csv.lzma
Fixed (| and \t)
Unpack from LZMA format

1. Poprawiono dane - dużo znaków '|' z doatkowymi tabulatorami/spacjami i trochę spacji zamiast tabulatorów pomiędzy.
2. W networkx klasa Graph przechowuje grafy nieskierowane
3. Zgodnie z https://networkx.github.io/documentation/networkx-2.0/reference/classes/generated/networkx.Graph.add_edge.html#networkx.Graph.add_edge dodanie krawędzi, która istnieje tylko nadpisuje istniejącą, więc nie ma zduplikowanych krawędzi.
4. Jest dużo powtarzających się węzłów (linii w pliku z danymi), a także dużo innych węzłów wzietych z dependencies. Kiedy któryś z węzłów istnieje, funkcja add_edge tylko go nadpisuje (nie usuwając przystających krawędzi), co tutaj nic nie zmienia. Kiedy nie istnieje, add_edge tworzy nowy węzeł -> stąd taka, a nie inna liczba węzłów

234844 / 3 = 78281 r. 1
Zadanie:
1.   wyznacz asortatywność średnią (8) i Pearsona (6); sporządź wykres danych użytych do identyfikacji tej ostatniej (3).

