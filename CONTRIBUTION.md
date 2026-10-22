# Contributing to Severn Trace 🚀

Thank you for taking the time to contribute to **Severn Trace**! Open-source contributions, feature suggestions, and bug reports help make this runtime and CLI faster, cleaner, and more valuable for developers worldwide.

---

## 🛠 Local Development Setup

To set up your local development environment and start testing changes:

1. **Fork and clone the repository:**
```bash
git clone https://github.com/YOUR_USERNAME/severn-trace.git
cd severn-trace

```


2. **Create and activate a virtual environment:**
```bash
python3 -m venv venv
source venv/bin/activate

```


3. **Install build tools and package in editable mode:**
```bash
pip install --upgrade pip build twine
pip install -e .

```



---

## 📐 Core Architecture Rules

To maintain the performance, security, and integrity of `severn-trace`, all code contributions must strictly adhere to these three core principles:

* **Zero External Dependencies:** No third-party packages may be added to `pyproject.toml` or runtime requirements. All utility functions, formatting, and time tracking must rely strictly on the Python standard library.
* **Minimal Overhead:** Diagnostic and tracing wrapper code must execute with minimal latency. Avoid heavy computations inside high-frequency trace hooks.
* **Type Annotations & Clean Syntax:** Ensure all new methods, classes, and CLI commands include full Python type hints and follow standard PEP 8 formatting.

---

## 📥 Submitting Pull Requests (PRs)

1. **Create a Feature Branch:**
```bash
git checkout -b feature/your-feature-name

```


2. **Commit Your Changes:**
Write clear, descriptive commit messages outlining what was modified or added.
3. **Push to Your Fork:**
```bash
git push origin feature/your-feature-name

```


4. **Open a Pull Request:**
Submit your PR against the `main` branch with a clear description of the problem solved or functionality added.
