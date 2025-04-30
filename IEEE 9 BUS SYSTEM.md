
- standardized benchmark model used extensively in power system studies. 
- It serves as a simplified representation of a real-world power grid, facilitating the analysis and validation of various power system concepts and tools.
- ![[Pasted image 20250430163624.png]]
- There are three generator subsystems in the model. Each of them comprises a synchronous machine and associated automatic voltage regulator (AVR), exciter, power system stabilizer (PSS), governor, and prime mover.
- Simscape™ Electrical™ first performs a load-flow analysis for the model and determines the steady-state operating point for a given loading condition. For each generator subsystem, you can use the initial load flow solution to determine the initial field circuit voltage and current value for the AVR and the initial torque value for the governor. To determine these initial conditions, right-click a synchronous machine block and select Electrical->Display Associated Initial Conditions. This prints the initial field circuit voltage, the initial field circuit current, and the initial mechanical torque in MATLAB® Command Window.
- The simulation then starts from this steady-state operating point. At time 10 s, an additional load is applied at Bus-6. After the simulation, the resulting load-flow solution is appended to each of the busbars.

- ### What does it comprise of?
	- 3 Generators: Representing power sources, each connected to a bus.​
	- 3 Loads: Simulating power consumption at different buses.
	- 9 Buses: Nodes where generators, loads, and transmission lines interconnect.​
	- 6 Transmission Lines: Facilitating power flow between buses
	- 3 Transformers: Adjusting voltage levels between different parts of the system.

---
References:
- [IEEE 9-Bus System](https://in.mathworks.com/help/sps/ug/ieee-9-bus.html)
- 