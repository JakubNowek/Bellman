# CMakeList.txt: projekt CMake dla elementu P2_Bellman, dołącz źródło i zdefiniuj
# tutaj logikę specyficzną dla projektu.
#
cmake_minimum_required (VERSION 3.8)

project ("P2_Bellman")
include_directories(inc)
file(GLOB SOURCE "src/*.cpp" "inc/*.hpp" "inc/*.h")
# Dodaj źródło do pliku "src/Bellman.cpp" tego projektu.
add_executable( ${PROJECT_NAME} ${SOURCE}  "inc/vector.hpp" "src/vector.cpp" "inc/graph.hpp" "inc/graph_list.hpp" "src/graph_list.cpp" "inc/graph_matrix.hpp" "src/graph_matrix.cpp" "inc/bellman_ford.hpp" "src/bellman_ford.cpp")

# TODO: Dodaj testy i zainstaluj elementy docelowe w razie potrzeby.
