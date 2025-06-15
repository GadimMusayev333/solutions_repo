## Problem 1 : 
\documentclass{article}
\usepackage{amsmath, amssymb}
\usepackage{graphicx}
\usepackage{geometry}
\geometry{margin=1in}
\title{Problem 1: Simulating the Effects of the Lorentz Force}
\date{}

\begin{document}

\maketitle

\section*{🎯 Motivation}

The Lorentz force equation:

$$
\vec{F} = q \vec{E} + q \vec{v} \times \vec{B}
$$

describes the force experienced by a charged particle in electric ($$\vec{E}$$) and magnetic ($$\vec{B}$$) fields. This fundamental law governs the behavior of charged particles in a wide range of physical systems, from particle accelerators and mass spectrometers to astrophysical plasmas and magnetic confinement devices in fusion research.

Simulating the motion of such particles enables visualization of their dynamic paths and a deeper understanding of phenomena like cyclotron motion, helical trajectories, and drift behavior in combined fields.

\section*{1️⃣ Exploration of Applications}

\subsection*{📌 Key Systems Influenced by Lorentz Force}
\begin{itemize}
  \item \textbf{Particle Accelerators}: Use $$\vec{E}$$ and $$\vec{B}$$ fields to bend and accelerate charged particles.
  \item \textbf{Mass Spectrometers}: Use $$\vec{B}$$ fields to separate ions by mass-to-charge ratio.
  \item \textbf{Plasma Confinement Devices (Tokamaks)}: Use $$\vec{B}$$ fields to confine hot plasma.
  \item \textbf{Cathode Ray Tubes (CRTs)}: Deflect electron beams using $$\vec{E}$$ and $$\vec{B}$$ fields.
  \item \textbf{Auroras and Cosmic Rays}: Charged particles spiral along Earth’s $$\vec{B}$$ field lines.
\end{itemize}

\subsection*{📌 Importance of Fields}
\begin{itemize}
  \item \textbf{Electric Field} ($$\vec{E}$$): Causes linear acceleration.
  \item \textbf{Magnetic Field} ($$\vec{B}$$): Causes circular or helical motion due to perpendicular force.
\end{itemize}

The cross product $$\vec{v} \times \vec{B}$$ ensures that the magnetic force is always perpendicular to the velocity.

\section*{2️⃣ Simulating Particle Motion (Conceptual Explanation)}

The motion of a particle of mass $$m$$ and charge $$q$$ under Lorentz force is governed by:

$$
m \frac{d\vec{v}}{dt} = q \vec{E} + q \vec{v} \times \vec{B}
$$

\subsection*{🔁 Case 1: Uniform Magnetic Field Only}

Set $$\vec{E} = 0$$

Then the force becomes:

$$
\vec{F} = q \vec{v} \times \vec{B}
$$

The particle moves in a circle in the plane perpendicular to $$\vec{B}$$.

\textbf{Larmor radius}:

$$
r = \frac{m v_\perp}{q B}
$$

\textbf{Cyclotron frequency}:

$$
\omega = \frac{q B}{m}
$$

\subsection*{🔁 Case 2: Uniform Electric and Magnetic Fields}

\textbf{If parallel} ($$\vec{E} \parallel \vec{B}$$): Spiral motion along field lines.

\textbf{If crossed} ($$\vec{E} \perp \vec{B}$$): E-cross-B drift occurs:

$$
\vec{v}_{\text{drift}} = \frac{\vec{E} \times \vec{B}}{B^2}
$$

Total motion = circular motion due to $$\vec{B}$$ + uniform drift due to $$\vec{E}$$.

\subsection*{🔁 Case 3: Electric Field Only}

Linear acceleration:

$$
\vec{a} = \frac{q \vec{E}}{m}
$$

\section*{3️⃣ Parameter Exploration}

\begin{center}
\begin{tabular}{|c|p{10cm}|}
\hline
\textbf{Parameter} & \textbf{Effect} \\
\hline
Electric Field ($$E$$) & Increases linear acceleration or drift. \\
\hline
Magnetic Field ($$B$$) & Decreases Larmor radius; increases cyclotron frequency. \\
\hline
Initial Velocity ($$v$$) & Affects radius or helical pitch. \\
\hline
Charge ($$q$$) & Reverses force direction if sign flips; magnitude affects curvature. \\
\hline
Mass ($$m$$) & Higher mass increases Larmor radius and slows rotation. \\
\hline
\end{tabular}
\end{center}

\section*{4️⃣ Visualization (Conceptually)}

\textbf{2D} motion under uniform $$\vec{B}$$: Circle in $$x$$–$$y$$ plane. \\
\textbf{3D} motion with $$v_z \ne 0$$: Helical trajectory.

With crossed $$\vec{E}$$ and $$\vec{B}$$ fields: Cycloidal path with drift velocity $$\vec{v}_{\text{drift}}$$.

\textbf{Key Concepts}:
\begin{itemize}
  \item \textbf{Larmor Radius}: $$r = \frac{m v_\perp}{q B}$$
  \item \textbf{Helical Pitch}: Depends on $$v_\parallel$$
  \item \textbf{Drift Velocity}: $$\vec{v}_{\text{drift}} = \frac{\vec{E} \times \vec{B}}{B^2}$$
\end{itemize}

\section*{✅ Real-World Connections}

\begin{center}
\begin{tabular}{|c|p{10cm}|}
\hline
\textbf{System} & \textbf{Lorentz Force Role} \\
\hline
Cyclotron & Circular motion from $$\vec{B}$$ and acceleration from $$\vec{E}$$. \\
\hline
Mass Spectrometer & Radius depends on $$\frac{mv}{qB}$$ for separation. \\
\hline
Magnetic Traps & Use magnetic fields to confine plasma. \\
\hline
Auroras & Particles spiral along Earth’s $$\vec{B}$$ and collide with atmosphere. \\
\hline
\end{tabular}
\end{center}

\section*{📌 Extension Ideas}
\begin{itemize}
  \item Add time-varying or non-uniform fields.
  \item Include inter-particle forces (e.g., Coulomb).
  \item Simulate collisions or external perturbations.
\end{itemize}

\section*{📤 Deliverables Summary}
\begin{itemize}
  \item \textbf{Markdown Document}: Theory + parameter analysis + applications.
  \item \textbf{Visualizations}: 2D and 3D trajectory plots.
  \item \textbf{Code (Optional)}: Euler/Runge-Kutta simulation of Lorentz force.
  \item \textbf{Discussion}: Physical implications and real-world relevance.
\end{itemize}

\end{document}
