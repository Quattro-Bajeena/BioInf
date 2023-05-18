Pytania:

- Czy możemy po prostu użyć algorytmu projesora Formanowicza?
- Czy do złożoności obliczeniowej liczy się także sama konstrukcja grafu?
- jak sprawdzać poprawność odpowiezi ze zbioru danych testowych?

Terminologia

- Lysov - słowo jest node
- Pevzner - słowo jest krawędzią
- SBH - sequencing by hybridization 
- NGS - next generation sequencing
- reads - słowa - oligonukleotydy


- Prof Błażewicz
  - Full graph (oligonukleotydy are nodes) with weights
  - heuristic,selective variant of TSP

- Overlap graphs
  - Lysov graphs, but oligonukleotydy can overlap only partially to have an edge between them.
  - weighted edges. weight function based on alignment score
  - heuristic approach to finding longest hamiltionian path
  - there may be none. but few dividing graph into few contigs

- Decomposition-based graphs
  - reads are decomposed into shorter k-mers
  - k-mers as arcs, between overlapping vertices like in Pevzner (exact matchings)
  - because there may be mutliple of a k-mer, it's a multigraph (or edges are labeled fe. 3 when there are 3 of that k-mer)
  - finding eulerian path. finding set of paths contating majority of edges at least once.

Wiemy jak skontruować graf. Czy zadaniem jest wymyślenie od zera heurystycznego algorytmu 