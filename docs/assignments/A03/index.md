# A3 – Parametric and FEA

## Objective

## Analyze

### Parametric Design

- Material: Aluminum
- Applied Load, F = 400 lbf
- Young's Modulus, E = 10,000,000 psi
- Maximum Axial Deflection, δ = 0.009 in
- Bar Diameter, d = 0.200 in
- Aluminum Yield Strength, Sy = 40 ksi

**Cross-Sectional Area**

A = πd² / 4

A = π(0.200 in)² / 4

A = 0.031415926536 in²

**Parametric Length Calculation**

δ = FL / AE

where:

- δ = axial deflection
- F = applied force
- L = bar length
- A = cross-sectional area
- E = Young's Modulus

The equation was rearranged to solve for the required length:

L = δAE / F

L = [(0.009 in)(0.031415926536 in²)(10,000,000 psi)] / (400 lbf)

L = 7.068583 in

**CAD Parameters and Equations**
<img width="563" height="344" alt="dimensions" src="https://github.com/user-attachments/assets/c8b9d71f-8123-40a1-93f7-0546a175944c" />

<img width="601" height="255" alt="CAD equations" src="https://github.com/user-attachments/assets/1ece52c3-ed21-4d1e-9b6e-4acabc65ee90" />

### Finite Element Analysis (FEA)

**Material Properties**
<img width="610" height="478" alt="Materials" src="https://github.com/user-attachments/assets/17d14003-399a-4916-bf47-938a2cdaf75d" />

A custom aluminum material was assigned with the following properties:

- Elastic Modulus = 10,000,000 psi
- Poisson's Ratio = 0.33
- Mass Density = 0.0975 lb/in³
- Yield Strength = 40,000 psi

I found the Poisson’s ratio and mass density by researching general material properties for aluminum and used the most appropriate values.

**Fixtures and Applied Load**
<img width="413" height="113" alt="forces" src="https://github.com/user-attachments/assets/ea179ea8-6806-4188-9354-f1838078fa20" />

**Mesh**
<img width="894" height="204" alt="mesh" src="https://github.com/user-attachments/assets/b1a3c90f-1a0b-4baa-afe9-4d5e710fa98d" />

**Deflection Map**

<img width="456" height="488" alt="deflection " src="https://github.com/user-attachments/assets/e72ec1f8-fbf2-4057-a70d-5b1acea911d9" />

**von Mises Stress Map**
<img width="434" height="478" alt="Stress" src="https://github.com/user-attachments/assets/c5702c2f-1013-4a3e-b971-afd3045ffa1b" />

**Maximum Stress and Safety Factor**

σ max = 13.47 ksi

Sy = 40 ksi

13.47 < 40 ✓

SF = Sy/σmax

SF = 40/13.47

SF = 2.97

### Design Analysis

**Percent Difference**

δ given = 0.009 in

δ FEA = 0.008993 in

% Difference = |δFEA - δhand| / δhand × 100

% Difference = |0.008993 - 0.009| / 0.009 × 100

% Difference = 0.0778%


**Pin-Hole Stress Concentration, Peak Stress, and Safety Factor**

d/H = 0.20

Kt ≈ 3.15

σ nominal = 12.68 ksi

σ peak = Kt(σnominal)

σ peak = (3.15)(12.68)

σ peak = 39.942 ksi

SF hole = Sy/σpeak

SF hole = 40/39.942

SF hole ≈ 1.00

SF hole < SF original

1.00 < 2.97

## Decide

### Design Reflection



## Communicate

### Lessons Learned

### Mistakes and Challenges

### Actual Time Spent

### CAD File Download
