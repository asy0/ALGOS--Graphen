# ALGOS--Graphen

Dieses Repository enthält Implementierungen von Graphalgorithmen in C und C++ mit einer CMake-basierten Build-Umgebung.

Highlights
- Implementationen gängiger Graphalgorithmen (BFS, DFS, Dijkstra, Bellman‑Ford, Floyd‑Warshall, Kruskal, Prim, Topologische Sortierung, SCC, Max-Flow usw.)
- C- und C++-Implementierungen für Vergleichszwecke
- CMake-Buildsystem für einfache Kompilierung und Tests
- Beispiele und kleine Benchmarks



Build-Anleitung (CMake)
1. Repository kopieren:
   ```bash
   git clone https://github.com/asy0/ALGOS--Graphen.git
   cd ALGOS--Graphen
   ```
2. Build-Verzeichnis anlegen und bauen:
   ```bash
   mkdir -p build
   cd build
   cmake ..
   cmake --build . --config Release
   ```
3. Tests ausführen (wenn eingerichtet):
   ```bash
   ctest --output-on-failure
   ```
4. Beispielprogramme aus `examples/` laufen lassen:
   ```bash
   ./examples/example_bfs
   ```

Beispiel: Kompilieren eines einzelnen Beispiels
```bash
# vom Projekt-Root aus
mkdir -p build && cd build
cmake ..
cmake --build . --target examples
./examples/example_dijkstra
```

Implementierte Algorithmen 
- Traversierung: BFS, DFS
- Kürzeste Wege: Dijkstra, Bellman‑Ford, Floyd‑Warshall
- Minimaler Spannbaum: Kruskal, Prim
- Ordnungen & Komponenten: Topologische Sortierung, Kosaraju, Tarjan (SCC)
- Flussalgorithmen: Edmonds‑Karp, Dinic
- Weitere Hilfsalgorithmen: Union-Find/Disjoint Sets, Priority Queue (Adapter)



- Verbesserte Benchmarks und Ergebnisvisualisierung
- Weitere Algorithmen (z. B. A*, Johnson)
- Dokumentation mit Diagrammen / Pseudocode
