# Problem 2
# Problem 2: Escape Velocities and Cosmic Velocities

## 🧠 Motivation

The concept of **escape velocity** is central to understanding how spacecraft leave a celestial body’s gravitational influence. Extending this idea, the **first**, **second**, and **third cosmic velocities** define the thresholds required to:

- Orbit a planet,
- Escape a planet’s gravity,
- Escape the entire Solar System.

These concepts underpin satellite launches, Moon and Mars missions, and future interstellar travel.

---

## 🚀 1. Definitions of the Cosmic Velocities

### 🟢 First Cosmic Velocity — *Orbital Velocity*

**Meaning**: The minimum horizontal velocity required for a stable circular orbit near the surface of a celestial body.

**Formula**: 
$$
\[
v_1 = \sqrt{\frac{GM}{R}}
\]
$$

---

### 🔵 Second Cosmic Velocity — *Escape Velocity*

**Meaning**: The minimum velocity needed to escape a planet’s gravitational field without further propulsion.

**Formula**:  
\[
v_2 = \sqrt{\frac{2GM}{R}} = \sqrt{2} \cdot v_1
\]

---

### 🔴 Third Cosmic Velocity — *Solar System Escape Velocity*

**Meaning**: The velocity required to escape the Sun’s gravitational field, starting from a planet’s orbital path.

**Formula (approximate)**:  
\[
v_3 = \sqrt{v_{\text{esc,Sun}}^2 + v_{\text{orb}}^2}
\]

Where:

- \[
v_{\text{orb}} = \sqrt{\frac{GM_{\odot}}{r}}
\]
- \[
v_{\text{esc,Sun}} = \sqrt{\frac{2GM_{\odot}}{r}}
\]

---

## 📐 2. Parameters Affecting These Velocities

- $G = 6.67430 \times 10^{-11} \, \text{m}^3/\text{kg}/\text{s}^2$ — gravitational constant  
- $M$ = Mass of the planet  
- $R$ = Radius of the planet  
- $M_{\odot} = 1.989 \times 10^{30} \, \text{kg}$ — Solar mass  
- $r$ = Distance from the Sun to the planet  

---

## 🧮 3. Manual Calculations of Cosmic Velocities

### 📊 Planetary Data

| Planet   | Mass (kg)           | Radius (m)         | Orbital Radius (m)     |
|----------|---------------------|--------------------|-------------------------|
| Earth    | $5.972 \times 10^{24}$ | $6.371 \times 10^6$ | $1.496 \times 10^{11}$ |
| Mars     | $6.417 \times 10^{23}$ | $3.390 \times 10^6$ | $2.279 \times 10^{11}$ |
| Jupiter  | $1.898 \times 10^{27}$ | $6.991 \times 10^7$ | $7.785 \times 10^{11}$ |

---

### 🌍 Earth

- First Cosmic Velocity:  
\[
v_1 = \sqrt{\frac{6.67430 \times 10^{-11} \cdot 5.972 \times 10^{24}}{6.371 \times 10^6}} \approx 7{,}905 \, \text{m/s}
\]

- Second Cosmic Velocity:  
\[
v_2 = \sqrt{2} \cdot v_1 \approx 11{,}180 \, \text{m/s}
\]

- Orbital Velocity:  
\[
v_{\text{orb}} = \sqrt{\frac{6.67430 \times 10^{-11} \cdot 1.989 \times 10^{30}}{1.496 \times 10^{11}}} \approx 29{,}780 \, \text{m/s}
\]

- Escape Velocity from Sun:  
\[
v_{\text{esc,Sun}} = \sqrt{2} \cdot v_{\text{orb}} \approx 42{,}100 \, \text{m/s}
\]

- Third Cosmic Velocity:  
\[
v_3 = \sqrt{(42{,}100)^2 + (29{,}780)^2} \approx 51{,}600 \, \text{m/s}
\]

---

### 🔴 Mars

- First Cosmic Velocity:  
\[
v_1 = \sqrt{\frac{6.67430 \times 10^{-11} \cdot 6.417 \times 10^{23}}{3.390 \times 10^6}} \approx 3{,}556 \, \text{m/s}
\]

- Second Cosmic Velocity:  
\[
v_2 = \sqrt{2} \cdot v_1 \approx 5{,}028 \, \text{m/s}
\]

- Orbital Velocity:  
\[
v_{\text{orb}} \approx 24{,}130 \, \text{m/s}
\]

- Escape Velocity from Sun:  
\[
v_{\text{esc,Sun}} \approx 34{,}100 \, \text{m/s}
\]

- Third Cosmic Velocity:  
\[
v_3 = \sqrt{(34{,}100)^2 + (24{,}130)^2} \approx 41{,}800 \, \text{m/s}
\]

---

### 🟠 Jupiter

- First Cosmic Velocity:  
\[
v_1 = \sqrt{\frac{6.67430 \times 10^{-11} \cdot 1.898 \times 10^{27}}{6.991 \times 10^7}} \approx 42{,}100 \, \text{m/s}
\]

- Second Cosmic Velocity:  
\[
v_2 = \sqrt{2} \cdot v_1 \approx 59{,}500 \, \text{m/s}
\]

- Orbital Velocity:  
\[
v_{\text{orb}} \approx 13{,}060 \, \text{m/s}
\]

- Escape Velocity from Sun:  
\[
v_{\text{esc,Sun}} \approx 18{,}460 \, \text{m/s}
\]

- Third Cosmic Velocity:  
\[
v_3 = \sqrt{(18{,}460)^2 + (13{,}060)^2} \approx 22{,}500 \, \text{m/s}
\]

---

## 📊 4. Summary Table

| Planet   | $v_1$ (m/s) | $v_2$ (m/s) | $v_3$ (m/s) |
|----------|-------------|-------------|-------------|
| Earth    | 7,905       | 11,180      | 51,600      |
| Mars     | 3,556       | 5,028       | 41,800      |
| Jupiter  | 42,100      | 59,500      | 22,500      |

---

## 🌠 5. Importance in Space Exploration

- **$v_1$ (First Cosmic Velocity)** is used for launching satellites into **Low Earth Orbit (LEO)**.
- **$v_2$ (Second Cosmic Velocity)** is needed to send missions to the **Moon, Mars**, and beyond.
- **$v_3$ (Third Cosmic Velocity)** is required to **leave the Solar System** — this was achieved by the **Voyager and Pioneer probes**.

Understanding these speeds helps engineers:

- Design rockets with sufficient **thrust** and **fuel efficiency**,
- Choose optimal **launch windows** and **paths**,
- Plan **interplanetary** and **deep space missions**.
