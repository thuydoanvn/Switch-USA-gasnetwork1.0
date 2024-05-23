SWITCH-GAS
______________________________________________________________________________________________________________________________

This repository has the modules and inputs for the SWITCH-GAS which was originally developed to study the efficiency of investment in natural gas network in the USA.

Modules extended by SWITCH-GAS should be solved with SWITCH 2.0, i.e. you need to install SWITCH2.0 first. These modules work with SWITCH2.0.7. Tutorials can be found at https://switch-model.org/. 
You may easily create a basic module to replace switch_model.timescales and switch_model.financials to make SWITCH-GAS a free-standing model based on Pyomo/Python language.

The "inputs" files serve as an example of inputs that can be used to run SWITCH-GAS model. Notes that it will take hours to solve the model with current input files. 
For a test run, you may want to reduce the input scale by either picking just few states or few timeseries. You can update corresponding data inputs to meet your modeling needs.

______________________________________________________________________________________________________________________________
The model developed in this paper possesses a structure that is similar to state-of-the-art capacity expansion models used for integration of renewable energy and storage in electricity systems. 
The model simultaneously optimizes investment decisions and operations decisions in order balance supply and demand on all days in all states, while satisfying import and export demands.  
We build the model using a mixed-integer linear-programming model, SWITCH 2.0, an open-soure platform for optimal capacity planning 
that thus far has focused on electric power systems. 

We modify the architecture to conform with gas networks. The optimization model minimizes the discounted total capital and operational cost of interstate pipeline, underground storage, 
and LNG facilities to meet the natural gas demand at each state in the 48 U.S. contiguous states and the District of Columbia. 

The main decision variables are necessary additional capacity of underground storage, LNG facilities, and state-to-state pipelines to accommodate the gas flow between supply and demand regions over the study period. 
In addition, the model computes optimal daily volume of natural gas injections into and withdrawals from underground storage, LNG facilities, as well as pipeline deliveries and receipts to meet the daily demand at each state. 

Constraints require that the total volume of natural gas from local production, net imports, net storage withdrawals, LNG regasification, and net pipeline receipts provides adequate natural gas for local consumption during on the daily basis. 
The amount of natural gas in underground storage, regasified from LNG, and transmitted through interstate pipeline are constrained by the capacity of underground storage, LNG facilities, and pipeline in each time period, respectively. 

This version of SWITCH-GAS takes **natural gas production (domestic supply), demand, imports from and exports to other countries as exogenous**. 

______________________________________________________________________________________________________________________________
Citation

Please cite the corresponding paper below to use the modules, data, and code of SWITCH-GAS:

Thuy Doan, Matthias Fripp, and Michael J. Roberts. 2022. "Are We Building Too Much Natural Gas Pipeline? A comparison of actual US expansion of pipeline to an optimized plan of the interstate network". 
The Economic Research Organization at the University of Hawaii. Working paper no.2022-2. https://uhero.hawaii.edu/wp-content/uploads/2022/04/UHEROwp2202.pdf

