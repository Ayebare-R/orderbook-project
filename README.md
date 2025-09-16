# C++ limit order book simulator
# Built in order to gain better understanding of how to build a trading system.

# To build:

```bash
cmake -S . -B build -DCMAKE_CXX_COMPILER=clang++
cmake --build build
./build/orderbook

# To run test:
ctest --test-dir build -V  


