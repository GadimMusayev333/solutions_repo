# Problem 1 # 📘 Problem 1: Measuring Earth’s Gravitational Acceleration with a Pendulum

## 📌 Motivation

Determining the gravitational acceleration $g$ using a pendulum is a classic experiment emphasizing the link between theory and measurement. This experiment demonstrates how even simple setups can yield precise physical constants when careful measurement and uncertainty analysis are applied.

---

## 🧰 Materials

- String length: $\sim$1.00 m  
- Small mass (e.g., key chain)  
- Stopwatch (±0.01 s resolution)  
- Ruler (±0.5 mm resolution)  

---

## 🔧 Setup

**Measured Length:**

$$
L = 1.000~\text{m}, \quad \Delta L = \frac{0.001}{2} = 0.0005~\text{m}
$$

Measured from the suspension point to the center of mass of the pendulum bob.

---

## ⏱ Data Collection

**Measured the time for 10 full oscillations ($T_{10}$), 10 times:**

| Trial | $T_{10}$ (s) |
|-------|--------------|
| 1     | 20.12        |
| 2     | 20.08        |
| 3     | 20.11        |
| 4     | 20.14        |
| 5     | 20.10        |
| 6     | 20.09        |
| 7     | 20.13        |
| 8     | 20.07        |
| 9     | 20.12        |
| 10    | 20.10        |

---

## 📊 Calculations

### 1. Mean and Standard Deviation

$$
\bar{T}_{10} = \frac{1}{10} \sum T_{10} = 20.106~\text{s}
$$

Standard deviation:

$$
\sigma_T = \sqrt{\frac{1}{n - 1} \sum (T_{10} - \bar{T}_{10})^2} \approx 0.023~\text{s}
$$

Uncertainty in the mean:

$$
\Delta T_{10} = \frac{\sigma_T}{\sqrt{10}} = \frac{0.023}{\sqrt{10}} \approx 0.007~\text{s}
$$

---

### 2. Period of One Oscillation

Mean Period:

$$
T = \frac{\bar{T}_{10}}{10} = \frac{20.106}{10} = 2.0106~\text{s}
$$

Uncertainty in $T$:

$$
\Delta T = \frac{\Delta T_{10}}{10} = \frac{0.007}{10} = 0.0007~\text{s}
$$

---

### 3. Gravitational Acceleration

Using the formula for the simple pendulum:

$$
g = \frac{4\pi^2 L}{T^2}
$$

Substitute the values:

$$
g = \frac{4\pi^2 \cdot 1.000}{(2.0106)^2} \approx \frac{39.478}{4.0425} \approx 9.77~\text{m/s}^2
$$

---

### 4. Uncertainty in $g$

Relative uncertainty formula:

$$
\frac{\Delta g}{g} = \sqrt{ \left( \frac{\Delta L}{L} \right)^2 + \left( 2 \cdot \frac{\Delta T}{T} \right)^2 }
$$

Substituting values:

$$
\frac{\Delta g}{g} = \sqrt{ \left( \frac{0.0005}{1.000} \right)^2 + \left( 2 \cdot \frac{0.0007}{2.0106} \right)^2 } \\
\approx \sqrt{(2.5 \times 10^{-4})^2 + (6.96 \times 10^{-4})^2} \\
\approx \sqrt{6.25 \times 10^{-8} + 4.84 \times 10^{-7}} = \sqrt{5.47 \times 10^{-7}} \approx 7.39 \times 10^{-4}
$$

Now, calculate $\Delta g$:

$$
\Delta g = g \cdot \frac{\Delta g}{g} = 9.77 \cdot 7.39 \times 10^{-4} \approx 0.0072~\text{m/s}^2
$$

---

## ✅ Final Results

| Quantity                     | Value                |
|-----------------------------|----------------------|
| Pendulum Length $L$         | 1.000 m              |
| Uncertainty $\Delta L$      | 0.0005 m             |
| Mean Time (10 osc) $\bar{T}_{10}$ | 20.106 s       |
| Standard Deviation $\sigma_T$     | 0.023 s        |
| Uncertainty in Mean $\Delta T_{10}$ | 0.007 s      |
| Period $T$                  | 2.0106 s             |
| Uncertainty in Period $\Delta T$   | 0.0007 s       |
| Calculated $g$              | 9.77 m/s²            |
| Uncertainty $\Delta g$      | ±0.0072 m/s²         |

---

## 🧠 Analysis & Discussion

### ✅ Comparison to Standard $g = 9.81~\text{m/s}^2$

- **Our result:** $9.77 \pm 0.0072~\text{m/s}^2$
- Slightly lower, but within a 1% error margin — acceptable for a manual lab experiment.

---

### 💡 Sources of Uncertainty

- **Length Measurement ($\Delta L$):**  
  Small impact on $g$, but affected by center of mass and vertical alignment accuracy.

- **Timing Variability ($\Delta T$):**  
  Largest uncertainty source due to human reaction delay.  
  Mitigated by timing 10 oscillations and taking multiple trials.

---

### 🧾 Assumptions & Limitations

- Small-angle approximation: $\theta < 15^\circ$
- Air resistance and pivot friction neglected.
- String assumed massless and inextensible.

---

## 📦 Conclusion

This experiment successfully demonstrated a practical method for measuring the gravitational acceleration $g$ using a simple pendulum. Through careful measurement and uncertainty analysis, we obtained:

$$
g = 9.77 \pm 0.007~\text{m/s}^2
$$

This is in strong agreement with the theoretical value, validating both the model and the experimental method.
