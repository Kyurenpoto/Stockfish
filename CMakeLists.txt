cmake_minimum_required(VERSION 3.17)
project(Stockfish)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set (CMAKE_CXX_EXTENSIONS OFF)
file(GLOB_RECURSE SRC "*.cpp")
add_executable(stockfish src/benchmark.cpp
src/bitbase.cpp
src/bitboard.cpp
src/endgame.cpp
src/evaluate.cpp
src/main.cpp
src/material.cpp
src/misc.cpp
src/movegen.cpp
src/movepick.cpp
src/pawns.cpp
src/position.cpp
src/psqt.cpp
src/search.cpp
src/thread.cpp
src/timeman.cpp
src/tt.cpp
src/uci.cpp
src/ucioption.cpp
src/tune.cpp
src/syzygy/tbprobe.cpp
src/nnue/evaluate_nnue.cpp
src/nnue/features/half_kp.cpp)