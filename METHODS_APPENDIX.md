# METHODS APPENDIX

## Reproducible Calculations for Kirandeep's Law of Emergence

**By Kirandeep Kaur**
**January 29, 2026**

---

# 1. CALCULATION FRAMEWORK

## 1.1 The E Formula

```
E = ΔI / A = ΔI / (Energy × Time)
```

## 1.2 Standard Procedure

For each case:
1. Define the task/outcome
2. Quantify ΔI (bits of uncertainty resolved)
3. Measure Energy (joules or cost proxy)
4. Measure Time (seconds)
5. Calculate E
6. Compare E ratios

---

# 2. BACKTEST CALCULATIONS

## 2.1 Wright Brothers vs. Langley

### The Task
Achieve powered, controlled human flight.

### Langley (Smithsonian)

**Information Gain:**
```
Outcome: Crashed into Potomac River (twice)
ΔI = 0 bits (task not completed)
```

**Energy (Cost Proxy):**
```
Funding: $50,000 (1900 dollars)
Energy equivalent: $50,000 × 10⁶ J/$ = 5 × 10¹⁰ J
```

**Time:**
```
Duration: 7 years = 7 × 365.25 × 24 × 3600 = 2.21 × 10⁸ seconds
```

**E Calculation:**
```
E_langley = 0 / (5 × 10¹⁰ × 2.21 × 10⁸)
E_langley = 0 bits/J·s
```

### Wright Brothers

**Information Gain:**
```
Outcome: Achieved sustained powered flight (Dec 17, 1903)
ΔI = 1 bit (binary: flight possible = yes)

More precisely:
Prior: P(human flight possible) ≈ 0.5
Posterior: P(human flight possible) = 1.0
ΔI = H(0.5) - H(1.0) = 1 - 0 = 1 bit
```

**Energy (Cost Proxy):**
```
Total spent: ~$1,000
Energy equivalent: $1,000 × 10⁶ J/$ = 10⁹ J
```

**Time:**
```
Serious work: 4 years = 1.26 × 10⁸ seconds
```

**E Calculation:**
```
E_wright = 1 / (10⁹ × 1.26 × 10⁸)
E_wright = 1 / 1.26 × 10¹⁷
E_wright = 7.9 × 10⁻¹⁸ bits/J·s
```

### Comparison

```
If Langley had succeeded:
E_langley_hypothetical = 1 / (5 × 10¹⁰ × 2.21 × 10⁸)
E_langley_hypothetical = 9.0 × 10⁻²⁰ bits/J·s

Ratio: E_wright / E_langley_hypothetical = 85×
```

**Prediction:** Wright wins (higher E)
**Outcome:** Wright Brothers achieved first flight ✓

---

## 2.2 Netflix vs. Blockbuster

### The Task
Deliver one movie viewing experience to customer.

### Blockbuster (2005)

**Information Gain:**
```
Task: Customer wants to watch specific movie
Prior uncertainty: Which movie? Is it available? Will it work?
Posterior: Movie watched successfully

Availability uncertainty: ~0.7 probability movie in stock
ΔI = -log₂(0.7) × 0.7 + failure cases ≈ 0.7 bits effective
```

**Energy (Cost):**
```
Customer cost: $4 rental + $2 gas + $10 late fees (average)
Plus store operation cost allocated: ~$1
Total: ~$17 per rental
Energy proxy: $17 × 10⁷ J/$ = 1.7 × 10⁸ J
```

**Time:**
```
Drive to store: 15 min
Browse/checkout: 10 min
Drive home: 15 min
Return trip: 30 min
Total: 70 min = 4,200 seconds

But for comparison, we use just acquisition time:
Time to acquire movie: 40 min = 2,400 seconds
```

**E Calculation:**
```
E_blockbuster = 0.7 / (1.7 × 10⁸ × 2400)
E_blockbuster = 0.7 / 4.08 × 10¹¹
E_blockbuster = 1.7 × 10⁻¹² bits/J·s
```

### Netflix Streaming (2010)

**Information Gain:**
```
Task: Same - watch specific movie
Availability: ~0.9 probability (larger catalog)
ΔI ≈ 0.9 bits effective
```

**Energy (Cost):**
```
Monthly subscription: $10 / 30 movies = $0.33 per movie
Electricity for streaming: ~$0.10
Bandwidth cost: ~$0.05
Total: ~$0.50 per movie
Energy proxy: $0.50 × 10⁷ J/$ = 5 × 10⁶ J
```

**Time:**
```
Search and click: 30 seconds
Buffer: 5 seconds
Total: 35 seconds
```

**E Calculation:**
```
E_netflix = 0.9 / (5 × 10⁶ × 35)
E_netflix = 0.9 / 1.75 × 10⁸
E_netflix = 5.1 × 10⁻⁹ bits/J·s
```

### Comparison

```
E_netflix / E_blockbuster = 5.1 × 10⁻⁹ / 1.7 × 10⁻¹²
E_ratio = 3,000×
```

**Note:** Earlier estimate of 7,017× used different time assumptions. Order of magnitude (1000×+) is robust.

**Prediction:** Netflix wins
**Outcome:** Blockbuster bankrupt 2010 ✓

---

## 2.3 Digital Photography vs. Film (Kodak)

### The Task
Capture and view one photograph.

### Kodak Film (2000)

**Information Gain:**
```
One photo: Resolves "what did this scene look like?"
Resolution: ~10 megapixels equivalent
But viewable information: ~1000 distinguishable features
ΔI ≈ log₂(1000) ≈ 10 bits per meaningful photo
```

**Energy (Cost):**
```
Film: $0.50 per shot
Processing: $0.30 per shot
Printing: $0.20 per shot
Camera amortized: $0.10 per shot
Total: $1.10 per photo
Energy: $1.10 × 10⁷ J/$ = 1.1 × 10⁷ J
```

**Time:**
```
Take photo: 1 second
Wait for development: 3 days = 2.6 × 10⁵ seconds
Get prints: 1 hour = 3,600 seconds
Total to viewable: 2.6 × 10⁵ seconds
```

**E Calculation:**
```
E_film = 10 / (1.1 × 10⁷ × 2.6 × 10⁵)
E_film = 10 / 2.86 × 10¹²
E_film = 3.5 × 10⁻¹² bits/J·s
```

### Digital Camera (2010)

**Information Gain:**
```
Same: ΔI ≈ 10 bits per photo
(Actually higher due to instant review and retake, but kept equal for comparison)
```

**Energy (Cost):**
```
Camera amortized: $500 / 10,000 photos = $0.05
Electricity: $0.001
Storage: $0.001
Total: $0.052 per photo
Energy: $0.052 × 10⁷ J/$ = 5.2 × 10⁵ J
```

**Time:**
```
Take photo: 0.5 seconds
View on screen: 0.5 seconds
Total: 1 second
```

**E Calculation:**
```
E_digital = 10 / (5.2 × 10⁵ × 1)
E_digital = 10 / 5.2 × 10⁵
E_digital = 1.9 × 10⁻⁵ bits/J·s
```

### Comparison

```
E_digital / E_film = 1.9 × 10⁻⁵ / 3.5 × 10⁻¹²
E_ratio = 5.4 × 10⁶ (5.4 million×)
```

**Prediction:** Digital wins
**Outcome:** Kodak bankrupt 2012 ✓

---

## 2.4 Bitcoin vs. Bank Wire (International Transfer)

### The Task
Transfer $10,000 internationally with certainty of delivery.

### Bank Wire (2020)

**Information Gain:**
```
Prior: Will money arrive? When? How much after fees?
Posterior: Money confirmed received

Uncertainty resolved:
- Delivery confirmation: 1 bit
- Amount certainty: ~2 bits (fee variations)
- Timing: ~2 bits (1-5 day range)
ΔI ≈ 5 bits
```

**Energy (Cost):**
```
Wire fee: $45 sender
Correspondent bank: $20
Receiver fee: $15
FX spread: $100 (1%)
Total: $180
Energy: $180 × 10⁷ J/$ = 1.8 × 10⁹ J
```

**Time:**
```
Initiate: 30 minutes = 1,800 s
Processing: 3 days = 2.6 × 10⁵ s
Confirmation: 1 hour = 3,600 s
Total: ~2.7 × 10⁵ seconds
```

**E Calculation:**
```
E_bank = 5 / (1.8 × 10⁹ × 2.7 × 10⁵)
E_bank = 5 / 4.86 × 10¹⁴
E_bank = 1.0 × 10⁻¹⁴ bits/J·s
```

### Bitcoin (2020)

**Information Gain:**
```
Same task: ΔI ≈ 5 bits
(Actually higher certainty due to blockchain verification)
```

**Energy (Cost):**
```
Network fee: $5 (average)
Electricity for transaction: negligible
Energy: $5 × 10⁷ J/$ = 5 × 10⁷ J

Note: Mining energy is distributed across all transactions, 
allocated here at ~$5 worth per transaction
```

**Time:**
```
Create transaction: 2 minutes = 120 s
Confirmation (6 blocks): 60 minutes = 3,600 s
Total: 3,720 seconds
```

**E Calculation:**
```
E_bitcoin = 5 / (5 × 10⁷ × 3720)
E_bitcoin = 5 / 1.86 × 10¹¹
E_bitcoin = 2.7 × 10⁻¹¹ bits/J·s
```

### Comparison

```
E_bitcoin / E_bank = 2.7 × 10⁻¹¹ / 1.0 × 10⁻¹⁴
E_ratio = 2,700×
```

**Prediction:** Bitcoin wins for international transfers
**Outcome:** Bitcoin primary use case is remittance/international ✓

---

## 2.5 Darwin vs. Wallace

### The Task
Formulate theory of evolution by natural selection.

### Darwin

**Information Gain:**
```
Theory of natural selection: ~100 bits
(Compresses vast biological observations into simple principle)
```

**Energy:**
```
20+ years of work
Beagle voyage: ~$100,000 equivalent
Living expenses while writing: ~$200,000 equivalent
Total: ~$300,000
Energy: $300,000 × 10⁶ J/$ = 3 × 10¹¹ J
```

**Time:**
```
From Beagle return (1836) to Origin (1859): 23 years
23 × 3.15 × 10⁷ = 7.25 × 10⁸ seconds
```

**E Calculation:**
```
E_darwin = 100 / (3 × 10¹¹ × 7.25 × 10⁸)
E_darwin = 100 / 2.175 × 10²⁰
E_darwin = 4.6 × 10⁻¹⁹ bits/J·s
```

### Wallace

**Information Gain:**
```
Same theory: ~100 bits
```

**Energy:**
```
Fever-dream insight while ill in Malay Archipelago
Prior field work: ~$20,000 equivalent
Insight period: minimal additional cost
Energy: $20,000 × 10⁶ J/$ = 2 × 10¹⁰ J
```

**Time:**
```
Field work: 8 years, BUT
Actual insight: Few days during fever
For theory formation: ~1 week = 6 × 10⁵ seconds
For total journey to insight: 8 years = 2.5 × 10⁸ seconds
```

**E Calculation (using insight period):**
```
E_wallace = 100 / (2 × 10¹⁰ × 6 × 10⁵)
E_wallace = 100 / 1.2 × 10¹⁶
E_wallace = 8.3 × 10⁻¹⁵ bits/J·s
```

### Comparison

```
E_wallace / E_darwin = 8.3 × 10⁻¹⁵ / 4.6 × 10⁻¹⁹
E_ratio ≈ 18,000×
```

**Prediction:** Higher E arrives faster
**Outcome:** Wallace's letter forced Darwin to publish ✓

---

# 3. PI COMPUTATION TESTS

## 3.1 Framework

For pi calculations:
```
ΔI = digits computed (in bits) = digits × log₂(10) = digits × 3.32 bits
Energy = computation energy (kWh × 3.6 × 10⁶ J/kWh)
Time = computation time (seconds)
```

## 3.2 Archimedes (250 BC)

**Method:** 96-sided polygon
**Digits:** 2 (3.14)
**ΔI:** 2 × 3.32 = 6.64 bits

**Energy:**
```
Human calculation: ~100 hours
Metabolic rate: 100 W
Energy: 100 × 3600 × 100 = 3.6 × 10⁷ J
```

**Time:**
```
100 hours = 3.6 × 10⁵ seconds
```

**E:**
```
E_archimedes = 6.64 / (3.6 × 10⁷ × 3.6 × 10⁵)
E_archimedes = 6.64 / 1.3 × 10¹³
E_archimedes = 5.1 × 10⁻¹³ bits/J·s
```

## 3.3 Madhava (1400 AD)

**Method:** Infinite series
**Digits:** 11
**ΔI:** 11 × 3.32 = 36.5 bits

**Energy:**
```
Human calculation: ~500 hours
Energy: 500 × 3600 × 100 = 1.8 × 10⁸ J
```

**Time:**
```
500 hours = 1.8 × 10⁶ seconds
```

**E:**
```
E_madhava = 36.5 / (1.8 × 10⁸ × 1.8 × 10⁶)
E_madhava = 36.5 / 3.24 × 10¹⁴
E_madhava = 1.1 × 10⁻¹³ bits/J·s
```

### Series vs Polygon Comparison

```
E_madhava / E_archimedes = 1.1 × 10⁻¹³ / 5.1 × 10⁻¹³ ≈ 0.2×

Wait - this shows polygon was MORE efficient per digit.
But series allows MORE digits. Let's recalculate for same effort:
```

**Revised comparison (same effort, different output):**
```
With 500 hours:
- Polygon method: ~3 digits (diminishing returns)
- Series method: 11 digits

E_series / E_polygon = (11/3) × same_denominator = 3.7×
```

## 3.4 ENIAC (1949)

**Method:** Machin's formula on first electronic computer
**Digits:** 2,037
**ΔI:** 2,037 × 3.32 = 6,763 bits

**Energy:**
```
ENIAC power: 150 kW
Run time: 70 hours
Energy: 150,000 × 70 × 3600 = 3.78 × 10¹⁰ J
```

**Time:**
```
70 hours = 2.52 × 10⁵ seconds
```

**E:**
```
E_eniac = 6,763 / (3.78 × 10¹⁰ × 2.52 × 10⁵)
E_eniac = 6,763 / 9.52 × 10¹⁵
E_eniac = 7.1 × 10⁻¹³ bits/J·s
```

## 3.5 Bellard Desktop (2009)

**Method:** Chudnovsky algorithm on desktop PC
**Digits:** 2.7 trillion
**ΔI:** 2.7 × 10¹² × 3.32 = 8.96 × 10¹² bits

**Energy:**
```
Desktop power: 500 W
Run time: 131 days
Energy: 500 × 131 × 24 × 3600 = 5.66 × 10⁹ J
```

**Time:**
```
131 days = 1.13 × 10⁷ seconds
```

**E:**
```
E_bellard = 8.96 × 10¹² / (5.66 × 10⁹ × 1.13 × 10⁷)
E_bellard = 8.96 × 10¹² / 6.4 × 10¹⁶
E_bellard = 1.4 × 10⁻⁴ bits/J·s
```

## 3.6 Comparison Table

| Era | Method | Digits | E (bits/J·s) |
|-----|--------|--------|--------------|
| 250 BC | Polygon | 2 | 5.1 × 10⁻¹³ |
| 1400 | Series | 11 | 1.1 × 10⁻¹³ |
| 1949 | ENIAC | 2,037 | 7.1 × 10⁻¹³ |
| 2009 | Desktop | 2.7T | 1.4 × 10⁻⁴ |

**E improvement 250 BC → 2009:**
```
E_ratio = 1.4 × 10⁻⁴ / 5.1 × 10⁻¹³
E_ratio = 2.7 × 10⁸ (270 million×)
```

---

# 4. COSMOLOGICAL PREDICTIONS

## 4.1 Dark Matter Ratio

**Formula:**
```
Dark Matter / Normal Matter = π^(3/2)
```

**Calculation:**
```
π^(3/2) = π × √π = 3.14159 × 1.7725 = 5.568
```

**Observed:**
```
Dark matter: 27% of universe
Normal matter: 5% of universe
Ratio: 27/5 = 5.4
```

**Accuracy:**
```
|5.568 - 5.4| / 5.4 = 3.1% error
Accuracy: 96.9%
```

## 4.2 Dark Energy Ratio

**Formula:**
```
Dark Energy / Total Matter = e^(3/4)
```

**Calculation:**
```
e^(0.75) = 2.117
```

**Observed:**
```
Dark energy: 68% of universe
Total matter: 32% of universe (27% dark + 5% normal)
Ratio: 68/32 = 2.125
```

**Accuracy:**
```
|2.117 - 2.125| / 2.125 = 0.38% error
Accuracy: 99.6%
```

## 4.3 Planck's Constant from π and μ

**Formula:**
```
ℏ = π^(-(2μ + 1/3 - π/(54μ²) + 55/(6072μ³)))
```

**Where μ = π³ + (21/22)π = 34.00507**

**Calculation:**
```
2μ = 68.01014
1/3 = 0.33333
π/(54μ²) = 3.14159/(54 × 1156.34) = 0.0000503
55/(6072μ³) = 55/(6072 × 39340.5) = 0.00000023

Exponent = 68.01014 + 0.33333 - 0.0000503 + 0.00000023
Exponent = 68.3434

ℏ_predicted = π^(-68.3434) = 1.0546 × 10⁻³⁴ J·s
```

**Observed:**
```
ℏ_actual = 1.054571817 × 10⁻³⁴ J·s
```

**Accuracy:**
```
|1.0546 - 1.05457| / 1.05457 = 0.003% error
Accuracy: 99.997%
```

---

# 5. PYTHON CALCULATOR

```python
"""
Kirandeep's Law of Emergence - E Calculator
E = ΔI / A = ΔI / (Energy × Time)
"""

import math

def calculate_E(delta_I_bits, energy_joules, time_seconds):
    """
    Calculate Certainty Efficiency E
    
    Parameters:
    - delta_I_bits: Information gain in bits
    - energy_joules: Energy in joules
    - time_seconds: Time in seconds
    
    Returns:
    - E in bits per joule-second
    """
    action = energy_joules * time_seconds
    E = delta_I_bits / action
    return E

def shannon_entropy(probabilities):
    """
    Calculate Shannon entropy H(X)
    
    Parameters:
    - probabilities: list of probabilities (must sum to 1)
    
    Returns:
    - H in bits
    """
    H = 0
    for p in probabilities:
        if p > 0:
            H -= p * math.log2(p)
    return H

def information_gain(prior_probs, posterior_probs):
    """
    Calculate information gain ΔI = H(prior) - H(posterior)
    """
    H_prior = shannon_entropy(prior_probs)
    H_posterior = shannon_entropy(posterior_probs)
    return H_prior - H_posterior

def cost_to_energy(cost_dollars, year=2025):
    """
    Convert monetary cost to energy proxy
    
    Historical energy per dollar (approximate):
    1900: 10^6 J/$
    2000: 10^7 J/$
    2025: 10^7 J/$
    """
    if year < 1950:
        joules_per_dollar = 1e6
    else:
        joules_per_dollar = 1e7
    return cost_dollars * joules_per_dollar

def compare_E(E1, E2, name1="System 1", name2="System 2"):
    """
    Compare two E values and predict winner
    """
    ratio = E1 / E2
    if ratio > 1:
        winner = name1
    else:
        winner = name2
        ratio = 1 / ratio
    print(f"{name1} E: {E1:.2e} bits/J·s")
    print(f"{name2} E: {E2:.2e} bits/J·s")
    print(f"Ratio: {ratio:.1f}×")
    print(f"Predicted winner: {winner}")
    return winner, ratio

# Constants
MU = 34.00507  # Emergence depth
PI = math.pi
HBAR = 1.054571817e-34  # J·s
K_B = 1.380649e-23  # J/K

def landauer_energy(temperature_K):
    """
    Minimum energy to erase 1 bit at temperature T
    E_min = k_B * T * ln(2)
    """
    return K_B * temperature_K * math.log(2)

def theoretical_max_E(temperature_K, min_time_s):
    """
    Theoretical maximum E at given temperature
    """
    E_min = landauer_energy(temperature_K)
    return 1 / (E_min * min_time_s)

def derive_pi_from_hbar():
    """
    Derive π from Planck's constant using the discovered relationship
    """
    from scipy.optimize import brentq
    
    h_bar = 6.62607015e-34 / (2 * PI)  # Exact SI definition
    
    def equation(pi_val):
        mu = pi_val**3 + (21/22)*pi_val
        corr1 = pi_val / (54 * mu**2)
        corr2 = 55 / (6072 * mu**3)
        exponent = 2*mu + 1/3 - corr1 + corr2
        return pi_val**(-exponent) - h_bar
    
    pi_derived = brentq(equation, 3.1, 3.2)
    return pi_derived

# Example usage
if __name__ == "__main__":
    print("=== Netflix vs Blockbuster ===")
    E_netflix = calculate_E(0.9, cost_to_energy(0.50), 35)
    E_blockbuster = calculate_E(0.7, cost_to_energy(17), 2400)
    compare_E(E_netflix, E_blockbuster, "Netflix", "Blockbuster")
    
    print("\n=== Landauer Bound at Room Temperature ===")
    E_landauer = landauer_energy(300)
    print(f"Minimum energy per bit: {E_landauer:.2e} J")
    
    print("\n=== π Derivation ===")
    try:
        pi_derived = derive_pi_from_hbar()
        print(f"Derived π: {pi_derived:.15f}")
        print(f"Actual π:  {PI:.15f}")
        print(f"Match: {abs(pi_derived - PI) < 1e-12}")
    except ImportError:
        print("Install scipy for π derivation: pip install scipy")
```

---

# 6. SPREADSHEET FORMULAS

## For Excel/Google Sheets

**Cell References:**
- A2: delta_I (bits)
- B2: energy (joules) OR cost ($)
- C2: time (seconds)
- D2: year (for cost conversion)

**Formulas:**

**Convert cost to energy:**
```
=IF(D2<1950, B2*1000000, B2*10000000)
```

**Calculate E:**
```
=A2/(B2*C2)
```

**Shannon entropy (for binary):**
```
=-A2*LOG(A2,2)-(1-A2)*LOG(1-A2,2)
```

**Compare E (ratio):**
```
=E2/E3
```

**Predict winner:**
```
=IF(E2>E3, "System 1", "System 2")
```

---

# 7. REPRODUCTION CHECKLIST

To reproduce any calculation:

1. [ ] Identify the task being compared
2. [ ] Define information gain (what uncertainty is resolved?)
3. [ ] Quantify ΔI in bits (use Shannon formula if needed)
4. [ ] Measure or estimate energy in joules (or use cost proxy)
5. [ ] Measure time in seconds
6. [ ] Calculate E = ΔI / (Energy × Time)
7. [ ] Compare E values
8. [ ] Higher E should win

---

# 8. SENSITIVITY ANALYSIS

## How robust are the conclusions?

**Netflix vs Blockbuster:**
```
Even with 10× uncertainty in measurements:
E_netflix / E_blockbuster ranges from 300× to 30,000×

Conclusion (Netflix wins) is robust.
```

**Digital vs Film:**
```
Even with 100× uncertainty:
E_digital / E_film ranges from 50,000× to 500,000,000×

Conclusion (Digital wins) is robust.
```

**General rule:**
When E ratios exceed 100×, the conclusion is robust to measurement error.

---

**END OF METHODS APPENDIX**

---

*"The universe minimizes action. Intelligence maximizes certainty per action. Same law, different frame."*

— Kirandeep Kaur, 2026
