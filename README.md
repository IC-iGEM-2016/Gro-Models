# Gro-Models
# Code written by Ecolibrium - Imperial iGEM team 2016

Description: This year, the Imperial iGEM team has decided to use a new language to visualise the behavior of its Genetically Engineered Artificial Ratio (G.E.A.R.) system: Gro. This new language, has allowed us to run hundreds of stochastic simulations, displayed as real-time animations, that provided us with an idea of how our system behaves. Gro proved to be a powerful visualisation tool that Matlab and its Simbiology toolbox both lacked. We have used this tool since the early stages of our project development to explain our circuit to scientists in Imperial College London and designers at the Royal College of Art. As a result Gro played a major role in the construction of our Visualisation Guidebook, which aims to help iGEM teams, particularly the ones on the foundation track, to communicate their project more clearly and efficiently to all kind of audiences. 

Gro, developed by the Klavins group at the University of Washington, simulates the behaviour of cells in microcolonies including intrinsic and extrinsic noise. In this way the platform allowed us to carry out stochastic modelling of a version of our circuit to simulate the multicellular behaviours we are expecting. 

The model we have produced is a high level model, designed to visually communicate the behaviour of our system at a population level. Due to a lack of computational power, the following simulations, unlike the Matlab models, do not include typical behaviour such as competition for resources, assuming infinite amount of resource and space for the cell populations. However all models by definition include diffusion rates so that we can explore this effect of population level behaviour on our circuit. The following simulations took an average of 2 days to run. 

To use the code download the gro programme from https://github.com/klavinslab/gro. We would like to thank Eric Klavins and James Macdonald for their help.

Final_Model.gro : this programme allows for stochastic modelling of our circuitry with paramaters found from either literature or estamated calculations. The programme is designed to run using the srand(-1) function allowing for a different run dependent on the time the run has started, therefore the programme was run 30 times in parallel.

financebanks.gro : this programme allows for stochastic modelling of a "financial model" where 3 banks are all dependent on one another using our system. As one bank crashes at 180 minutes, due to the nature of the circuit the other two populations survive. The programme is designed to run using the srand(-1) function allowing for a different run dependent on the time the run has started, therefore the programme was run 30 times in parallel.

financebankscontrol.gro : this programme allows for stochastic modelling of a "financial control model" where 3 banks are all dependent on one another via an auxotrophic system. As one bank crashes at 180 minutes, due to the nature of the auxotrophic control the population dependent on the crashed population also dies and hence the third dies too. The programme is designed to run using the srand(-1) function allowing for a different run dependent on the time the run has started, therefore the programme was run 30 times in parallel.

Without Circuit : This programme allows for stochastic modelling of a control to show growth of two populations without any circuitry implemented. The programme is designed to run using the srand(-1) function allowing for a different run dependent on the time the run has started, therefore the programme was run 30 times in parallel.
