## 📘 Numerical Methods — Bisection Method Task (NMAL-01)

**Assigned Date**: `22/06/2025`  
**Task Code**: [Display Text](NAML-01.py)

---

### ✅ Task Objectives

1. What could be the better approach to choose the range in the bisection method?  
2. Apply the technique to solve a problem:  
   - i) Traditional bisection method  
   - ii) Improved bisection method (with automatic interval selection)  
3. Compare performance by number of iterations  

---

### 🔍 1. Choosing a Better Range for Bisection

#### 📌 Traditional Approach
- Manually pick an interval \([a, b]\)
- Check if \( f(a) \cdot f(b) < 0 \)
- Success depends on lucky guessing

#### 💡 Improved Approach
- Use a graph or automate interval detection:
  - Loop over \([x, x + \delta]\)
  - Check if \( f(x) \cdot f(x + \delta) < 0 \)
  - If yes, use \([x, x + \delta]\) as the root interval

✅ This avoids guesswork and ensures a valid range is found.

---

### 🧪 2. Implementation

#### i) Traditional Bisection
- Fixed user-defined interval
- Stops when error \( < \epsilon \)

#### ii) Improved Bisection
- Automatically detects valid interval before applying bisection
- More reliable when root position is unknown

---

### ⚙️ Sample Test

- Enter start of the interval: 0
- Enter end of the interval: 5
- Enter the step size for scanning: 0.1
- Enter the error tolerance: 0.001
- Traditional bisection root: 1.5216064453125, iterations: 12
- Improved bisection root: 1.5210937500000004, iterations: 6


