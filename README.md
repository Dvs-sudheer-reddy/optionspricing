# Options Pricing — Black‑Scholes (C++)

A compact, readable C++ implementation of the Black‑Scholes option pricing model with a small demo program. This repository is ideal for students, quants, and engineers who want a clear, self-contained reference implementation.

## Features

- Clean implementation of the Black‑Scholes formula for European call and put options
- Accurate Normal CDF helper with a standalone implementation
- Small demo `Main.cpp` showing usage and simple CLI interaction
- Minimal dependencies: plain C++ (works with `g++` or MSVC)

## Files

- `BlackScholes.h` / `BlackScholes.cpp`: core pricing functions
- `NormalCDF.h` / `NormalCDF.cpp`: normal cumulative distribution helper
- `Main.cpp`: tiny demo runner to exercise the library

## Quick Start — Build

Compile with a recent C++ compiler (Linux / macOS / Windows with MinGW/MSYS or WSL):

```bash
g++ -std=c++17 -O2 -o black_scholes Main.cpp BlackScholes.cpp NormalCDF.cpp
```

Or with MSVC (Developer Command Prompt):

```powershell
cl /std:c++17 /O2 Main.cpp BlackScholes.cpp NormalCDF.cpp
```

## Run

After building, run the demo program:

```bash
./black_scholes
```

The program provides a simple interactive example. You can also integrate the library into your own project by including `BlackScholes.h` and calling the pricing functions directly.

## Example (conceptual)

Compute a European call option price using typical parameters:

- Underlying price: 100
- Strike price: 100
- Time to maturity (years): 0.5
- Risk-free rate: 0.01
- Volatility (sigma): 0.2

The demo program prints the computed call and put prices for such inputs.

## Why this repo?

- Educational: small, well-separated modules make it easy to follow the math and the code.
- Practical: drop-in functions for quick prototyping and verification of pricing logic.

## Next steps (ideas)

- Add unit tests and CI (GitHub Actions)
- Add more option models (e.g., implied volatility solver, Black‑76, local vol)
- Provide worked examples and Jupyter notebooks for visualization

## License

MIT — feel free to reuse and adapt. Contributions welcome.

---

If you'd like, I can add a quick example run, unit tests, or CI workflow next.
