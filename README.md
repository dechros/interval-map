# interval-map

Header-style `interval_map<K, V>` built on `std::map`, storing a value for each half-open key interval with an initial value for everything below the first boundary. Supports `assign(keyBegin, keyEnd, val)` and `operator[]` lookup while keeping adjacent equal-valued intervals merged.

## Layout

```
source/    interval_map.cpp, main.cpp
output/    build output
```

## Build

Requires C++17. Using g++:

```bash
g++ -std=c++17 -g source/*.cpp -o output/main
```

Run `./output/main` (or `output\main.exe` on Windows).
