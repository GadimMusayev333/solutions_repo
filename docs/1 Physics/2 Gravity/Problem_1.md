# Problem 1
# Kepler’s Third Law for Circular Orbits

## 1. Derivation of Kepler’s Third Law for Circular Orbits

For a body of mass $m$ orbiting a much larger mass $M$ in a circular orbit of radius $r$, the gravitational force provides the centripetal force required for circular motion:

$$
F_{\text{gravity}} = F_{\text{centripetal}} \Rightarrow \frac{G M m}{r^2} = \frac{m v^2}{r}
$$

Canceling $m$ and rearranging:

$$
v^2 = \frac{G M}{r}
$$

The orbital period $T$ is the time to complete one full circle:

$$
T = \frac{2\pi r}{v}
$$

Substitute $v$:

$$
T = \frac{2\pi r}{\sqrt{\frac{G M}{r}}} = 2\pi \sqrt{\frac{r^3}{G M}}
$$

**Final Relationship**:

$$
T^2 = \frac{4\pi^2}{G M} r^3
$$

This is **Kepler's Third Law for circular orbits**:

$$
T^2 \propto r^3
$$

---

## 2. Implications for Astronomy

- **Planetary Masses**: If $T$ and $r$ are known for a satellite, we can estimate the mass $M$ of the central body.
- **Orbital Prediction**: The law helps determine the position and motion of planets and moons.
- **Exoplanet Studies**: Kepler’s Law helps detect exoplanets through variations in orbital periods.

---

## 3. Real-World Examples

### Moon Orbiting the Earth

- $r = 3.84 \times 10^8$ m  
- $T = 27.3$ days $ \approx 2.36 \times 10^6$ s

Use the law to find Earth’s mass:

$$
M = \frac{4\pi^2 r^3}{G T^2}
$$

### Planets in the Solar System

For each planet:

$$
\frac{T^2}{r^3} \approx \text{constant}
$$

This confirms Kepler’s Law.

---

## 4. Computational Simulation (Python)

```python
import numpy as np
import matplotlib.pyplot as plt

# Constants
G = 6.67430e-11  # m^3 kg^-1 s^-2
M = 1.989e30     # mass of the Sun in kg

# Orbital radii (m)
radii = np.linspace(0.2, 30, 100) * 1.496e11  # from 0.2 to 30 AU

# Orbital periods (s)
periods = 2 * np.pi * np.sqrt(radii**3 / (G * M))

# Convert to years
periods_years = periods / (60 * 60 * 24 * 365.25)

# Plot T^2 vs r^3
plt.figure(figsize=(8, 5))
plt.plot(radii**3, periods**2, label=r'$T^2$ vs $r^3$')
plt.xlabel(r'Orbital Radius Cubed $r^3$ (m$^3$)')
plt.ylabel(r'Orbital Period Squared $T^2$ (s$^2$)')
plt.title('Kepler\'s Third Law: $T^2 \\propto r^3$')
plt.grid(True)
plt.legend()
plt.tight_layout()
plt.show()
