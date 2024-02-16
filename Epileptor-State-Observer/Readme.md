# Epileptor Model - State Observer Design

This code was developed for the thesis entitled: "A contribution to the dynamics of epilepsy: identification and control for seizure attenuation" and then used for the following publication in Neural Computation:

Brogin, J. A. F., Faber, J., & Bueno, D. D. (2021). Burster reconstruction considering unmeasurable variables in the Epileptor model. Neural Computation, 33(12), 3288-3333.

which can be cited as:

@Article{Brogin2021burster,
  author   = {Brogin, João Angelo Ferres and Faber, Jean and Bueno, Douglas Domingues},
  journal  = {Neural Computation},
  title    = {{Burster Reconstruction Considering Unmeasurable Variables in the Epileptor Model}},
  year     = {2021},
  issn     = {0899-7667},
  month    = {11},
  number   = {12},
  pages    = {3288-3333},
  volume   = {33},
  doi      = {10.1162/neco_a_01443},
  eprint   = {https://direct.mit.edu/neco/article-pdf/33/12/3288/1972026/neco\_a\_01443.pdf},
  url      = {https://doi.org/10.1162/neco\_a\_01443},
}

The code was developed on the Spyder platform and consists of four separate files: “LMIs for designing an FTS observer for the Epileptor Model.py” is an optimization routine for computing the gains of the fuzzy Takagi-Sugeno state observer for the Epileptor model based on Linear Matrix Inequalities (LMIs); “Observer approach for the Epileptor model using a fourth-order Runge-Kutta integrator.py” uses the computed ganis in a closed-loop routine for estimating the unmeasurable states based on the measurable ones of the seizures described by the Epileptor model using the fourth-order Runge-Kutta integrator; “LMIs for designing an FTS controller for the mass-spring-damper example model.py” is an optimization routine for the mass-spring-damper system of one degree of freedom to illustrate the efficiency of the parameter beta, proposed in aforementioned paper; “Control approach for the mass-spring-damper model using a fourth-order Runge-Kutta integrator.py” uses the computed gains in a closed-loop routina for controlling the mass-spring-damper system using the fourth-order Runge-Kutta integrator.

To cite these codes in their respective ordem, please use the models in the files: “LMIs for designing an FTS observer for the Epileptor Model.cff”; “Observer approach for the Epileptor model using a fourth-order Runge-Kutta integrator.cff”; “LMIs for designing an FTS controller for the mass-spring-damper example model.cff”; “Control approach for the mass-spring-damper model using a fourth-order Runge-Kutta integrator.cff”.

Figure: The first file computes the gains of the fuzzy Takagi-Sugeno controller via Linear Matrix Inequalities (LMIs); the second file imports the gains from the first one and applies them along with the fourth-order Runge-Kutta integrator to reconstruct the unmeasurable states of the Epileptor model.
