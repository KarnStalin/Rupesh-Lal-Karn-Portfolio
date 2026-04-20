# TGA Kinetics Modeling: Thermal Decomposition Analysis

## Objective
To determine the kinetic parameters governing thermal decomposition using multi-rate thermogravimetric analysis (TGA) and isoconversional modeling methods.

---

## Experimental Framework

Thermal analysis was performed under controlled conditions using multiple heating rates:

- Heating rates (β): 5, 10, 20 °C/min  
- Atmosphere: Inert (e.g., nitrogen)  
- Measurement: Mass loss vs temperature  

---

## Conceptual Basis

## Conceptual Basis

Thermal decomposition follows:

$$
\frac{d\alpha}{dt} = k(T) f(\alpha)
$$

Where:
- α = conversion fraction  
- k(T) = temperature-dependent rate constant  
- f(α) = reaction model  

Arrhenius relation:

$$
k(T) = A e^{-E_a / RT}
$$

## Conversion Definition

## Conversion Definition

$$
\alpha = \frac{m_0 - m_t}{m_0 - m_f}
$$

Where:
- m₀ = initial mass  
- mₜ = mass at time t  
- m_f = final mass  

## Kinetic Modeling Methods

### 1. Kissinger Method

### 1. Kissinger Method

$$
\ln\left(\frac{\beta}{T_p^2}\right) = -\frac{E_a}{R T_p} + C
$$

- Uses peak temperature (Tₚ) at different heating rates  
- Provides apparent activation energy (Eₐ)  
- Assumes single-step dominant reaction  

---

### 2. Flynn–Wall–Ozawa (FWO) Method

:contentReference[oaicite:4]{index=4}

- Isoconversional method (constant α)  
- Does not require reaction model  
- Evaluates Eₐ across conversion range  

---

### 3. Kissinger–Akahira–Sunose (KAS) Method

$$
\ln\left(\frac{\beta}{T^2}\right) = -\frac{E_a}{RT} + C
$$
- Similar to FWO but uses different approximation  
- Provides more accurate Eₐ trends  

---

## Modeling Workflow

1. Perform TGA at multiple heating rates  
2. Extract conversion (α) vs temperature  
3. Identify peak temperature (Tₚ) for each β  
4. Apply Kissinger method for global Eₐ  
5. Apply FWO and KAS for conversion-dependent Eₐ  
6. Analyze variation of Eₐ with α  

---

## Key Insights

- Activation energy varies with conversion → indicates multi-step reaction behavior  
- Single-value Eₐ (Kissinger) may oversimplify complex systems  
- Isoconversional methods reveal underlying reaction complexity  
- Thermal stability is governed by multiple overlapping processes  

---

## Interpretation Strategy

- Compare Eₐ trends across samples  
- Identify distinct decomposition stages  
- Correlate kinetic parameters with:
  - Structural features  
  - Surface chemistry  
  - Porosity and morphology  

---

## Tools Used

- MATLAB: Kinetic modeling and regression  
- Python: Data extraction and processing  
- Origin: Plotting and fitting  

---

## Research Significance

This approach enables extraction of physically meaningful kinetic parameters without assuming a predefined reaction model, providing deeper insight into thermal decomposition mechanisms.

---

## Research Note

All numerical data and plots are excluded due to ongoing publication preparation. This section focuses on modeling methodology and interpretation framework.
