TIE-ABM: AI-Driven Smart-Green Manufacturing Ecosystem Simulation
Overview
This repository contains the source code, data, and documentation for a multi-agent simulation model built in NetLogo, as described in the research paper "From Efficiency Tool to Ecosystem Catalyst: The Evolutionary Study of AI-Driven Smart Manufacturing Ecosystems". The model implements a Technology-Institution-Ecology (TIE) synergistic evolution framework to explore how Artificial Intelligence (AI) drives the transition of manufacturing systems from individual optimization to ecosystem-level symbiosis under fiscal constraints.
The simulation integrates four types of agents—Manufacturers, Suppliers, Government, and Geographical Environment—to study the dynamic interplay of AI technological advancement, policy interventions, and ecological transformation. Key mechanisms include AI generational leaps, knowledge spillovers, green spatial diffusion, dynamic subsidies, and counter-cyclical transition fund releases, which collectively drive system-level self-organization and resilience.
This repository aims to ensure transparency and reproducibility of the research, allowing users to replicate the simulation, explore specific mechanisms, or extend the model for further studies.
Theoretical Foundation
The model is grounded in Complex Adaptive Systems (CAS) theory, integrating insights from evolutionary economics and institutional analysis. It simulates a 33×33 spatial grid representing a provincial-scale industrial park or urban cluster, with a time horizon of 500 ticks (approximately 40 years, where 1 tick = 1 month). The TIE framework captures:
Technology: AI as an "ecosystem catalyst" driving efficiency optimization, knowledge diffusion, and demand creation.
Institution: Dynamic policy mechanisms (e.g., green subsidies, carbon taxes, transition funds) ensuring fiscal sustainability via "exit-oriented governance."
Ecology: Spatial diffusion of green areas, reflecting the transition to sustainable manufacturing clusters.
Key emergent phenomena include non-linear demand expansion, cluster formation, and system resilience under external shocks.

Repository Contents
code/: Contains the NetLogo model file (TIE_ABM.nlogo) implementing the simulation.
data/: Includes initialization datasets, parameter calibration files, and sample output data for validation.
docs/: Supplementary documentation, including:
Detailed variable definitions (see Appendix A of the paper).
Pseudocode for core algorithms (see Appendix B of the paper).
Data sources and calibration methods (see Appendix C of the paper).
figures/: Visualizations of simulation results (e.g., evolution trajectories, spatial heatmaps).


Getting Started
Prerequisites
NetLogo: Version 6.4.0 or higher (download from NetLogo official website).
Basic understanding of agent-based modeling and NetLogo syntax.

Installation

Clone the repository:
bashgit clone https://github.com/wsmlxqa/TIE-ABM-AI-Driven-Smart-Green-Manufacturing-Ecosystem-Simulation/tree/main
Open code/TIE_ABM.nlogo in NetLogo.
Ensure any required data files from the data/ directory are properly linked in the NetLogo model.

Running the Simulation

1.Open the NetLogo model (TIE_ABM.nlogo).
2.Load the initial parameters from data/initial_params.csv or use the default settings as described in Table 2 of the paper.
3.Press the Setup button to initialize the model with:
50 Manufacturers, 100 Suppliers, and a 33×33 grid.
Initial green area ratio: 20%.
Base demand: 1000 units.
4.Press the Go button to run the simulation for 500 ticks.
5.Monitor key outputs (e.g., green coverage ratio, average AI generation, market price) via NetLogo's interface or export to data/output/ for analysis.

Simulation Scenarios
The model supports five key scenarios as described in Section 5 of the paper:
1.Baseline: Self-organized evolution without policy intervention.
2.Tech Dividend: High vs. low technology dividend effects on non-linear demand growth.
3.Policy Intervention: Static subsidies vs. dynamic fund vs. mixed policy.
4.External Shock: System resilience under a 25% competitiveness loss at t=200.
5.Spatial Evolution: Green area diffusion from scattered points to regional clusters.
To replicate these scenarios, adjust the relevant parameters (e.g., demand-beta, green-subsidy, disruption-prob) in the NetLogo interface or configuration files.

Reproducibility
To ensure reproducibility:
The NetLogo code is fully documented with comments aligning with the pseudocode in Appendix B.
All parameters are calibrated using real-world data (e.g., MIIT reports, McKinsey 2021) as detailed in Appendix C.
Sample output data and visualization scripts are provided in data/ and figures/ for comparison with the paper's results (e.g., Figures 1–5).


Case Study Validation
The simulation results are corroborated by real-world cases, including:
Haier COSMOPlat: AI-driven platform growth and carbon footprint reduction.
CATL: Non-linear demand surge post-CTP battery technology breakthrough.
Sany Heavy Industry: Resilience via AI-optimized "lighthouse factory" during COVID-19.
Yangtze Delta Cluster: Spatial evolution of green manufacturing clusters.
These cases align with the model’s predictions of non-linear demand growth, spatial clustering, and system resilience.
Contributing
Contributions to improve the model, add new scenarios, or refine visualizations are welcome! Please:
Fork the repository.
Create a feature branch (git checkout -b feature/YourFeature).
Commit changes (git commit -m 'Add YourFeature').
Push to the branch (git push origin feature/YourFeature).
Open a Pull Request.

Citation
If you use this model in your research, please cite the original paper:
Juan Yu. (2025). From Efficiency Tool to Ecosystem Catalyst: The Evolutionary Study of AI-Driven Smart Manufacturing Ecosystems. 

Contact
For questions or feedback, open an issue on this repository.
