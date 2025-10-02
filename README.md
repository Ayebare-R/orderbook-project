# C++ Limit Order Book Simulator

This project is a high-performance C++ simulator for a financial limit order book (LOB). 

I built this to explore the core mechanics of market exchanges and to provide a robust framework for implementing and testing algorithmic trading strategies.

The simulator includes a C++ implementation of the Avellaneda-Stoikov market-making model, which dynamically adjusts bid and ask quotes based on factors like inventory risk and market volatility.

---

## Features

* **Complete Order Management**: Full support for limit orders, market orders, and cancellations.
* **Performance Tracking**: Real-time Profit and Loss (PnL) calculation for simulated strategies.
* **Data Logging**: Comprehensive logging of all trade fills and periodic order book snapshots to CSV files for later analysis.
* **Top-of-Book Queries**: Efficiently query the current best bid and ask prices.
* **Advanced Strategy Implementation**: Includes baseline market-making and the Avellaneda-Stoikov market-making model.

---

## Getting Started

### Prerequisites

* **CMake** (version 3.10 or higher)
* A modern C++ compiler that supports C++17 (e.g., **Clang++**, **GCC**)

### Build Instructions

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-directory>
    ```

2.  **Configure and build the project using CMake:**
    ```bash
    # Create a build directory
    cmake -S . -B build -DCMAKE_CXX_COMPILER=clang++

    # Compile the project
    cmake --build build
    ```

### Running the Simulator

Execute the main application from the project's root directory:

```bash
./build/orderbook
