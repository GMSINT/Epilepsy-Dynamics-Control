# Epileptor Control

This code was developed for the thesis entitled: "A contribution to the dynamics of epilepsy: identification and control for seizure attenuation" and then used for the following publication in the Journal of Neural Systems:

Brogin JAF, Faber J, Bueno DD. An Efficient Approach to Define the Input Stimuli to Suppress Epileptic Seizures Described by the Epileptor Model. Int J Neural Syst. 2020 Nov;30(11):2050062. doi: 10.1142/S0129065720500628. Epub 2020 Sep 16. PMID: 32938259.

which can be cited as:
@Article{brogin2020,
  author   = {Brogin, João Angelo Ferres and Faber, Jean and Bueno, Douglas Domingues},
  journal  = {International Journal of Neural Systems},
  title    = {An Efficient Approach to Define the Input Stimuli to Suppress Epileptic Seizures Described by the Epileptor Model},
  year     = {2020},
  note     = {PMID: 32938259},
  number   = {11},
  pages    = {2050062},
  volume   = {30},
  doi      = {10.1142/S0129065720500628},
  eprint   = {https://doi.org/10.1142/S0129065720500628},
  url      = {https://doi.org/10.1142/S0129065720500628},
}

The code was developed on the Spyder platform and it consists two separate files: LMIs_Epileptor.py is an optimization routine for computing the gains of the fuzzy Takagi-Sugeno controller based on the concept of Linear Matrix Inequalities (LMIs); Control_approach_Epileptor_RK4.py uses the computed gains in a closed-loop routine to suppress the seizures described by the Epileptor model using the fourth-order Runge-Kutta algorithm. 

To cite these codes in their respective order, please use the models in the files: “LMIs for designing an FTS controller for the Epileptor Model.cff”; “Control approach for the Epileptor model using a fourth-order Runge-Kutta integrator.cff”.

Figure: The first file computes the gains of the fuzzy Takagi-Sugeno controller via Linear Matrix Inequalities (LMIs); the second file imports the gains from the first one and applies them along with the fourth-order Runge-Kutta integrator to control the seizures described by the Epileptor model.
