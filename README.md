# severn-trace
severn-trace is a zero-dependency Python tracing SDK and execution runtime for autonomous AI agents.


 `README.md` structured specifically for `severn-trace`.





# Severn Trace (severn-trace) ⚡

[![PyPI Version](https://img.shields.io/pypi/v/severn-trace.svg)](https://pypi.org/project/severn-trace/)
[![Python Versions](https://img.shields.io/pypi/pyversions/severn-trace.svg)](https://pypi.org/project/severn-trace/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Severn Trace** is a ultra-lightweight, zero-dependency Python tracing runtime and CLI designed for deep execution visibility, function timing, and real-time debugging—without the bloat of standard heavyweight APM tools.

Built for high-performance Python environments, microservices, and rapid local diagnostic workflows.

---

## 🌟 Key Features

* Zero Third-Party Dependencies: Pure Python standard library implementation for zero footprint, lightning-fast boot times, and effortless auditability.
* Global CLI Diagnostics: Install via `pipx` or standard `pip` to access the global `severn` CLI directly from your shell.
* Low-Overhead Execution Tracing: High-precision telemetry for execution flow, runtime metrics, and performance bottlenecks.
* Seamless Integration: Simple, clean decorator and contextual APIs for rapid integration into existing codebases.

---

## 🚀 Quick Start & Installation

### Option 1: Global Installation (Recommended for CLI usage)
To use `severn` globally across your system without virtual environment conflicts, install via `pipx`:

```bash
pipx install severn-trace

```

### Option 2: Project Virtual Environment

To use `severn-trace` inside your Python project:

```bash
pip install severn-trace

```

---

## 💻 Usage & Code Examples

### 1. Basic Function Decorator

Wrap any critical function to automatically trace its execution time, call stack, and diagnostic metadata:

```python
from severn import trace

@trace
def process_data(records):
    # Your processing logic here
    total = sum(records)
    return total

if __name__ == "__main__":
    process_data([10, 20, 30, 40])

```

### 2. Global CLI Usage

Run performance diagnostics directly against your Python scripts from the command line:

```bash
severn run your_script.py



## Why Severn Trace?

Heavy APM agents like Datadog or New Relic add unnecessary memory overhead and complex setup for local execution analysis and microservices. `severn-trace` gives software engineers and founders instant visibility with zero external setup, keeping runtime overhead near zero.

---

## 🛠 Local Development & Setup

If you want to contribute to `severn-trace` or run it locally from source:

1. Clone the repository:
```bash
git clone [https://github.com/YOUR_USERNAME/severn-trace.git](https://github.com/YOUR_USERNAME/severn-trace.git)
cd severn-trace



2. Set up a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate

```


3. Install development dependencies and build tools:
```bash
pip install --upgrade pip build twine



4. Build package distribution:
```bash
python -m build




## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.


