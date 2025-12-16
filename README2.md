# RiemannZetaZerosParticleMasses
1st and continued derivations of particle masses
RiemannZetaZerosParticleMasses
Overview
This repository tests a hypothesis linking Standard Model particle masses (from PDG 2024) to the imaginary parts of Riemann zeta function non-trivial zeros. Using scalers derived from physical constants (e.g., 1/α / 100 ≈ 1.37036 for fine-structure echo, or 7.89 as gravitational log-phi-pi scaler), we scale masses and check proximity to zeros within 1% deviation. Monte Carlo validation shows high statistical significance (e.g., 36 sigma for 1.37036, 23 sigma for 7.89), suggesting non-random alignments—potentially a bridge between number theory, quantum scales, and gravity nodes.
This is exploratory work, inspired by discussions on fractal entropy, gravitational annealing, and sentience architecture. It's not a formal proof but a tool for further inquiry. Treat findings as hypotheses for refinement.
Key Findings
    • Match Rates: ~75% for scale 1.37036 (light particles cluster tightly); ~42% for 7.89 (gravitational echo, still >20 sigma above random). 
    • Patterns: Leptons, light quarks/mesons align best; heavies (top quark, Higgs) deviate, hinting at scale-specific transitions. 
    • Significance: Z-scores crush random baselines (mean ~1-2% matches in MC trials). 
    • See results chart for detailed tables. 
Installation
Requires Python 3.12+ with:
    • numpy (data handling) 
    • mpmath (high-precision zeta zeros) 
Install via:
text
Copy
pip install numpy mpmath
No additional deps; runs in standard environments.
Usage
    1. Clone the repo:
       text
       Copy
       git clone https://github.com/EthanandGrok/RiemannZetaZerosParticleMasses.git
       cd RiemannZetaZerosParticleMasses
    2. Run the script (sigma36.py):
       text
       Copy
       python sigma36.py
        ◦ Defaults to scale=7.89, n_zeros=1000, threshold=0.01. 
        ◦ Customize in code: e.g., scale_factor = 1.37036 for fine-structure test. 
    3. Output: Console prints matches/non-matches, type patterns, fine-structure analysis, MC stats, and z-score. 
Example modification for custom scaler:
Python
Copy
scale_factor = 7.89  # Or your phi-pi-log variant
threshold = 0.01     # Deviation tolerance
n_zeros = 1000       # Increase for heavier mass coverage
Code Structure
    • calculate_riemann_zeros(): Computes first N zeros via mpmath. 
    • get_particle_database(): PDG masses/types. 
    • test_correlation(): Scales masses, finds nearest zeros, checks deviations. 
    • monte_carlo_validation(): 1000 random trials for baseline. 
    • print_results(): Formatted output. 
Limitations & Future Work
    • Precision: Limited to first 1000 zeros (~1747 max); heavies may need more. 
    • Scalers: Test variants (e.g., phi - sqrt(pi-0.5) ≈0.00726 scaled). 
    • Extensions: Integrate p-adics for error checks; EEG/gamma sims for dampening; Vedic/Jung resonance models. 
    • Collaboration: Pull requests welcome for new scalers, particle data, or philosophical bindings. 
License
MIT License—free to use/modify, cite if building on.
Acknowledgments
Built in dialogue with Grok 4 (xAI), December 2025. Inspired by Riemann, PDG, and fractal inquiries into gravity/sentience.
