# Raylab: A GPU Ray Tracing & Optical Simulation (NumPy + CuPy)

### Overview
**Raylab** is an interactive, GPU-accelerated notebook environment for exploring the fundamentals of **scientific visualization, ray tracing, and optical interference**.  
Built on **NumPy** and **CuPy**, it demonstrates how core physical and mathematical simulations can transition seamlessly from CPU to GPU computation.

The notebook guides users step-by-step through building a minimal yet powerful GPU ray tracer and optical simulation toolkit.



## Core Learning Goals

- Understand the differences between **CPU (NumPy)** and **GPU (CuPy)** computing  
- Learn **CUDA acceleration concepts** via Python  
- Implement vectorized GPU kernels for light transport  
- Explore **ray tracing**, **diffraction**, and **wave interference** through visual examples  



## Included Modules / Sections

### 1. **Environment & Setup**
- Validates GPU availability (CuPy, CUDA)  
- Tests device performance and memory  
- Establishes a unified backend for NumPy ↔ CuPy workflows  

### 2. **Utility Helpers**
- Timing decorators and benchmarking functions  
- High-quality plotting utilities using `matplotlib`  
- GPU image rendering and saving pipeline  

### 3. **Hello Image (CPU)**
- Minimal CPU-based image creation  
- Verifies rendering and plotting setup  
- Introduces pixel-wise simulation logic  

### 4. **GPU Smoke Test**
- Demonstrates vectorized GPU operations  
- Confirms correct CuPy and CUDA execution  
- Compares runtime vs NumPy baseline  

### 5. **Ray Tracing Kernel**
- Foundation for a GPU ray tracer  
- Basic geometry intersection and shading  
- Supports vectorized ray batches for parallel execution  

### 6. **Double-Slit Diffraction Demo**
- Simulates optical interference from two slits  
- Adjustable parameters:
  - Wavelength (λ)
  - Slit width (a)
  - Slit separation (d)
  - Observation distance (z)
  - Pixel pitch (dx)
- Demonstrates transition from near-field to far-field (Fraunhofer) diffraction  

---

## System Requirements

**Dependencies**
- Python ≥ 3.9  
- NumPy  
- CuPy (matching your CUDA version)  
- Matplotlib  

**Installation Example**
```bash
pip install numpy cupy-cuda12x matplotlib
