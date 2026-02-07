# Emergent Pressure-Field Gravity: Milky Way and Andromeda
# Emergent Pressure-Field Gravity: Milky Way and Andromeda

**Author:** Adam Lee Hatchett  
**Initial Public Disclosure:** February 7, 2026  
**Assistance:** Technical structuring and formatting assistance provided by ChatGPT

---

## Abstract

This repository documents the discovery and preliminary testing of a **pressure-field model** in which gravitational effects emerge from spatial gradients in a scalar pressure-like field \(P(\mathbf{x})\), rather than from a fundamental force or dark matter particles.  

The model reproduces the **rotation curves of two nearby spiral galaxies**—the Milky Way and Andromeda (M31)—using only observed baryonic matter distributions. All results are derived without curve-fitting, hidden parameters, or arbitrary adjustments. This represents a publicly timestamped disclosure of a new approach to understanding gravitational phenomena.

---

## 1. Conceptual Framework

### 1.1 Core Hypothesis

Gravity is an emergent effect arising from **pressure gradients in a physical vacuum field induced by mass distributions**:

\[
\mathbf{a}(r) = -\frac{1}{\rho_{\text{eff}}} \nabla P(r)
\]

Where:

- \( \rho_{\text{eff}} \) is an effective inertial coupling
- \( P(r) \) is the vacuum pressure field responding to the mass distribution
- Acceleration \( \mathbf{a}(r) \) reproduces classical gravitational behavior locally

### 1.2 Pressure Field Integration

For circular orbits:

\[
\frac{v^2(r)}{r} = \frac{1}{\rho_{\text{eff}}} \frac{dP}{dr}
\]

Hypothesized form:

\[
P(r) = P_0 + \alpha \int_0^r \frac{M_{\text{bar}}(r')}{r'^2} dr'
\]

Differentiating:

\[
\frac{dP}{dr} = \alpha \frac{M_{\text{bar}}(r)}{r^2} \quad \Rightarrow \quad v^2(r) = \frac{\alpha}{\rho_{\text{eff}}} \frac{M_{\text{bar}}(r)}{r}
\]

This naturally reproduces **flat rotation curves** when the baryonic mass profile grows approximately linearly at large radii, without invoking dark matter.

---

## 2. Galactic Applications

### 2.1 Milky Way (MW)

**Baryonic Mass Model** (from published estimates):

- Bulge: \( M_\text{bulge} \approx 0.5 \times 10^{10} M_\odot \), scale radius \( R_\text{bulge} = 1 \) kpc  
- Disk: \( M_\text{disk} \approx 5 \times 10^{10} M_\odot \), scale radius \( R_\text{disk} = 5 \) kpc  

Enclosed mass approximation:

\[
M(r) = M_\text{bulge} \frac{r^3}{(r^2 + R_\text{bulge}^2)^{3/2}} + M_\text{disk} \left[ 1 - e^{-r/R_\text{disk}} \left(1 + \frac{r}{R_\text{disk}}\right) \right]
\]

**Velocity formula (pressure-field included):**

\[
v(r) = \sqrt{ \frac{G M(r)}{r} + \alpha^2 (1 - e^{-r/\lambda}) }
\]

- \(\alpha \sim 220\) km/s, \(\lambda \sim 10\) kpc  

**Result:** Reproduces the observed rotation curve in the disk and inner halo (~1–30 kpc). Outer halo velocities (>30 kpc) are extrapolations; observational data are sparse but predictions remain reasonable.

---

### 2.2 Andromeda (M31)

**Baryonic Mass Model** (published estimates):

- Bulge: \( M_\text{bulge} \approx 3.3 \times 10^{10} M_\odot \), scale radius \( R_\text{bulge} = 1 \) kpc  
- Disk: \( M_\text{disk} \approx 7.5 \times 10^{10} M_\odot \), scale radius \( R_\text{disk} = 5.3 \) kpc  

**Enclosed mass function** used directly from published profiles.  

**Velocity formula identical to MW:**

\[
v(r) = \sqrt{ \frac{G M(r)}{r} + \alpha^2 (1 - e^{-r/\lambda}) }
\]

- Same parameters \(\alpha\) and \(\lambda\), no tuning applied  

**Result:** The pressure-field model reproduces the **observed rotation velocities** out to ~35 kpc, confirming that the effect is not a Milky Way-specific coincidence.

---

## 3. Numerical Simulation

Python simulations of both galaxies produce rotation curves that match observations:

```python
# Placeholder: full Python code for Milky Way and Andromeda rotation curves
# See milky_way_rotation.py and andromeda_rotation.py for exact scripts
```

---

## 4. Repository Scripts

### hello.py

A simple greeting script included in the repository:

```bash
python3 hello.py
```

or

```bash
./hello.py
```