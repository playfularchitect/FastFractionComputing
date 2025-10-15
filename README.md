# WarpFrac — High-Performance GPU Fraction Arithmetic

WarpFrac is a Python library providing GPU-accelerated arithmetic for fractions using pre-compiled, high-performance CUDA kernels. This is a **binary-only evaluation release** and is not open-source.

---

## Performance Benchmarks

The following benchmarks were recorded on an **NVIDIA A100 (sm_80)** GPU.

| Operation | Tera-Operations/s (TOPS) | Giga-Operations/s (GOPS) |
| :-------- | :----------------------- | :----------------------- |
| **ADD** | `0.495`                  | `494.6`                  |
| **MUL** | `1.298`                  | `1297.3`                 |

---

## Requirements

* An NVIDIA GPU with one of the following compute capabilities:
    * **sm_75** (Turing Architecture, e.g., RTX 20-series)
    * **sm_80** (Ampere Architecture, e.g., A100)
    * **sm_86** (Hopper Architecture, e.g., H100)
* Python 3.x
* NVIDIA CUDA Toolkit compatible with your driver.
(You need Linux, if have mac use the colab stuff!)
---

## Installation 

1.  Navigate to the [Releases page](link-to-your-releases-page).
2.  Download the wheel file (`.whl`) and the checksum file (`.sha256`).
3.  (Optional) Verify the integrity of the download:
    ```bash
    sha256sum -c warpfrac-2025.10.14.1855-py3-none-any.whl.sha256
    ```
4.  Install the wheel using pip:
    ```bash
    pip install warpfrac-2025.10.14.1855-py3-none-any.whl
    ```

---

## Usage

### Command-Line Demo

Run a quick performance benchmark from your terminal:
```bash
warpfrac-demo
```

### Programmatic API

Use WarpFrac directly in your Python scripts. The functions return a dictionary containing performance metrics (`ops`, `sec`, `gops`, `tops`).

```python
import warpfrac as wf

# Run the addition benchmark
add_results = wf.headline_add()
print(f"Addition results: {add_results}")

# Run the multiplication benchmark
mul_results = wf.headline_mul()
print(f"Multiplication results: {mul_results}")
```

---

## License & Terms of Use

This software is distributed under a binary-only license. **Source code is not available, and reverse engineering, decompiling, or disassembling the binaries is strictly prohibited.**

* Please see the `LICENSE.txt` file for copyright information.
* Refer to `EULA.txt` for the full End-User License Agreement.
* **Note**: External publication of benchmarks requires prior written consent from me, Evan Wesley, The Smartest Idiot Alive.
