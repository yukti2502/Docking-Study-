
# In-silico Screening of Phytochemicals from Aloe barbadensis and Allium sativum Against Monkeypox Virus A42R Protein

## Overview
This project investigates the therapeutic potential of phytochemicals derived from *Aloe barbadensis* (Aloe vera) and *Allium sativum* (Garlic) against the A42R profilin-like protein of the Monkeypox virus (MPXV) using computational approaches. The study used molecular docking, MM-GBSA binding free energy calculation, and ADME profiling to identify natural compounds with promising antiviral properties.

---

## Key Highlights
- **Target Protein**: A42R profilin-like protein (PDB ID: 4QWO)
- **Ligand Source**: 91 phytochemicals from *Aloe barbadensis* and *Allium sativum* (IMPPAT database)
- **Tools Used**:
  - Schrödinger Suite (Maestro, LigPrep, Glide SP, SiteMap, Prime MM-GBSA, QikProp)
- **Top Hits**:
  - Sativoside B1 from *Allium sativum*: Docking Score = −7.80 kcal/mol
  - Isoaloesin from *Aloe barbadensis*: Docking Score = −5.29 kcal/mol
- **MM-GBSA Binding Energies**: Ranged from −47.20 to −18.54 kcal/mol
- **ADME Properties**: All top compounds met Lipinski’s Rule of Five and showed good pharmacokinetic profiles

---

## Methodology

### 1. Selection and Preparation of Ligands
- 91 phytochemicals were retrieved in 3D SDF format from the IMPPAT database.
- Ligand preparation was performed using LigPrep (Schrödinger Maestro Suite v13.2.138).
- Bond orders were assigned and ionization states generated.

### 2. Protein Preparation
- Target protein A42R profilin-like protein (PDB ID: 4QWO) was downloaded from the PDB.
- Water molecules, hydrogens, and metal ions were removed.
- Bond orders were assigned using the Protein Preparation Wizard.

### 3. Binding Site Prediction and Grid Generation
- SiteMap module was used to predict the binding site due to lack of known binding site.
- Sites with score > 0.9 were selected. Best site score: 1.004
- Grid box dimensions: 20 x 20 x 20 Å centered on Site 1.

### 4. Molecular Docking (Glide SP)
- All 91 ligands were docked using Glide’s Standard Precision (SP) mode.
- 14 compounds showed high binding affinity.

### 5. MM-GBSA Analysis
- MM-GBSA (via Prime) calculated free binding energy using 5 Å residue distance.
- Binding energies ranged from −35 to −18 kcal/mol, confirming stability.

### 6. In-silico ADME Profiling
- Top compounds analyzed using QikProp for ADME properties.
- Lipinski’s Rule of Five, QPlogS, QPlogBB, and %Human Oral Absorption evaluated.

---

## Results

### 1. Docking Scores (Glide SP)

| Plant              | Compound Name         | Docking Score (kcal/mol) |
|--------------------|------------------------|---------------------------|
| *Allium sativum*   | Sativoside B1          | **−7.80**                 |
| *Allium sativum*   | Eruboside B            | −6.98                     |
| *Allium sativum*   | Protojujuboside B      | −6.93                     |
| *Allium sativum*   | Sativoside R2          | −6.52                     |
| *Aloe barbadensis* | Isoaloesin             | −5.29                     |
| *Aloe barbadensis* | Aloesin                | −5.20                     |
| *Aloe barbadensis* | Chrysophanol           | −5.14                     |
| *Aloe barbadensis* | L-Rhamnose             | −5.04                     |
| *Aloe barbadensis* | Galactomannan          | −4.97                     |
| *Aloe barbadensis* | Emodin                 | −4.89                     |
| *Aloe barbadensis* | d-Tartaric acid        | −4.82                     |


---

### 2. MM-GBSA Binding Energies
| Compound              | Source Plant       | MM-GBSA Energy (kcal/mol) |
|-----------------------|--------------------|----------------------------|
| Protoeruboside B      | Allium sativum     | -39.48                     |
| Riboflavin            | Allium sativum     | -47.20                     |
| Protopine             | Allium sativum     | -42.24                     |
| Galactomannan         | Aloe barbadensis   | -35.87                     |
| Isoaloesin            | Aloe barbadensis   | -31.49                     |

<img width="550" height="550" alt="Screenshot (631)" src="https://github.com/user-attachments/assets/55d9a7c7-1a8d-4c21-a6e4-6188409cb59c" />
<img width="550" height="550" alt="Screenshot (632)" src="https://github.com/user-attachments/assets/58700628-aa84-4c70-9bbd-6701e1781e26" />
<img width="550" height="550" alt="Screenshot (633)" src="https://github.com/user-attachments/assets/c256bfa8-0b35-41d3-beab-a12e4a3649d2" />
<img width="550" height="550" alt="Screenshot (634)" src="https://github.com/user-attachments/assets/2ff9f874-3289-4607-8924-f2c46caf970e" />
<img width="550" height="550" alt="Screenshot (635)" src="https://github.com/user-attachments/assets/aea09a95-f98c-4b51-96c9-c774da2580ab" />


### 3. ADME Results (via QikProp)

| Compound       | Mol Wt. | Rule of 5 | QPlogS | QPlogBB | % Oral Absorption |
|----------------|---------|-----------|--------|---------|--------------------|
| Chrysophanol   | 254.24  | 0         | -2.90  | -0.99   | 80.60              |
| Isoaloesin     | 410.37  | 0         | -2.37  | -2.85   | 42.43              |
| Emodin         | 270.24  | 0         | -3.06  | -1.54   | 68.12              |
| L-Rhamnose     | 164.15  | 0         | -0.94  | -0.94   | 61.24              |
| Galactomannan  | 504.44  | 3         | -0.77  | -4.30   | 0.00               |

---

## Conclusion
This project successfully identifies phytochemicals from *Aloe barbadensis* and *Allium sativum* that show promising inhibitory interaction with the Monkeypox A42R protein. Compounds like **protoeruboside B** and **isoaloesin** exhibited strong docking and binding energy scores along with favorable pharmacokinetic properties. Further **in vitro/in vivo** experiments are needed for validation.

---

## Authors
- Yukti Sabikhi (yukti257@gmail.com)  
- Anshika Singh (anshikasingh090304@gmail.com)
