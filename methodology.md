# Methodology

## Calculations

> All metrics in cm or kg unless otherwise specified.

### Anthropometric Measurements

**Sitting Height (cm)**

```text
Sitting Height = Sitting Height - Bench Height
```

**Leg Length (cm)**

```text
Leg Length = Height - Sitting Height
```

---

### Maturity Calculations

**Maturity Offset (M.O.) [1]**

```text
−9.236 + 0.0002708×(Leg Length × Sitting Height)
− 0.001663×(Age × Leg Length)
+ 0.007216×(Age × Sitting Height)
+ 0.02292×(Height / Weight)
```

**Growth Rate (GrRt) (cm/yr)**

```text
linear regression slope across all of a player's height measurements.
```

**Peak Height Velocity Age (PHVA) [1]**

```text
PHVA = Age − Maturity Offset
```

---

### Predicted Adult Height

**Midparent Height (cm)**

```text
(Father Height + Mother Height) / 2
```

**Predicted Adult Height (cm) [2]**

```text
(β0 + β1×Height (in) + β2×Weight (lb) + β3×Midparent Height (in)) × 2.54
```

```text
multiplying by 2.45 converts back to cm.
```

Where:

```text
β0 = Intercept
β1 = Stature (Height) coefficient (in)
β2 = Weight coefficient
β3 = Midparent coefficient
```

```text
Coefficients are looked up from nearest matching age row in Coefficients table.
```

---

### Biological Maturation Classification

**Biological Age**

```text
Biological Age = Age + Maturity Offset
```

**Maturation Group**

```text
Biological Age - Age

> 1 = Early
< -1 = Late
otherwise Average [3]
```

---

### Additional Classifications

**Bio-band (PHV Stage) [4]**

**Growth Rate Flags (broadly applied) [5]**

---

## References

**[1]**

Mirwald, R.L., Baxter-Jones, A.D.G., Bailey, D.A., & Beunen, G.P. (2002). *An assessment of maturity from anthropometric measurements*. Medicine & Science in Sports & Exercise, 34(4), 689–694.

**[2]**

Khamis, H.J., & Roche, A.F. (1995). *Erratum: Predicting adult stature without using skeletal age*. Pediatrics, 95(3), 457.

**[3]**

Malina, R.M., Bouchard, C., & Bar-Or, O. (2004). *Growth, Maturation, and Physical Activity* (2nd ed.). Human Kinetics.

**[4]**

Cumming, S.P., Lloyd, R.S., Oliver, J.L., Eisenmann, J.C., & Malina, R.M. (2017). *Bio-banding in sport: applications to competition, talent identification, and strength and conditioning of youth athletes*. Strength and Conditioning Journal, 39(2), 34–47.

**[5]**

Malina, R.M., Bouchard, C., & Bar-Or, O. (2004). *Growth, Maturation, and Physical Activity* (2nd ed.). Human Kinetics.

