Assignment 6 β Thermal time response Sensor Physics 2022
Sakari Lukkarinen & Saana Vallius Metropolia University of Applied Sciences Instructions
First solve either problem 1 (easier) OR problem 2 (harder).
Then solve all the rest of the problems (3-5). Problem 1. (Easier)
Use pen and paper and verify by differentiation that π=π +(πβπ )βπ
where Tβ is temperatureβs rate of change.
Use the following numerical values for the solution:
Use paper and pen and verify by separation of variables that
Use the following numerical values for the solution:
π(0) = 20 Β°C, π = 100 Β°C, and π = 0.10 1.
Tip 1: The first step in separation is the following: ππ = βπ β ππ‘ (πβπ )
πππ£
Tip 2: Review Engineering Mathematics lecture notes.
πππ£ 0 πππ£
βππ‘
 is a solution for the Newtonβs law of cooling differential equation
β²
π=βπ(πβπ )
π(0)=20Β°C,π =100Β°C,andπ=0.10 1 πππ£ π 
Tip 1: First replace all symbols with their numerical values in the equations. Then differentiate the solution for π, substitute πβ and π into the Newtonβs law of cooling differential equation and simplify it to see that both sides are equal.
Tip 2: Review Engineering Mathematics lecture notes. Problem 2. (Harder)
π(π‘)=π +(πβπ )βπ πππ£ 0 πππ£
ππ‘
πππ£
πππ£
πππ£ π 
βππ‘
 is a solution for the Newtonβs law of cooling differential equation
ππ=βπ(πβπ )
 
Problem 3.
Sketchagraphofthesolutionπ(π‘)=π +(π βπ )βπ usingthegiven
Use pen and paper, Scientific Python, Excel, or any other tool you are familiar with to calculate the values and plot the graph.
Problem 4.
In thermal systems, the thermal rate π can be expressed as
πππ£ 0 πππ£
βππ‘
numerical values π(0) = 20 Β°C, π = 100 Β°C, and π = 0.10 1 in the range π‘ = 0 ... 60 π  πππ£ π 
π= hπ΄,where πΆπ‘ππ‘
- h is the heat transfer coefficient between the system and the environment,
- π΄ is the surface area of the system, and
- πΆπ‘ππ‘ is the total heat capacity of the system.
 The total heat capacity πΆπ‘ππ‘ can be represented by its mass-specific heat capacity πΆπ multiplied by its mass π πΆπ‘ππ‘ = πΆπ β π
 So, the thermal rate π becomes to
Find the thermal rate, if the system has the following properties
h=150 π ,π΄=590ππ2,π=0.76π,andπΆ =730 π½ π2πΎ π πππΎ
π= hπ΄ πΆππ
Sketch a graph of the temperature for the system following Newtonβs law of cooling (problems 1-3) for
π‘ = 0 ... 30 π , π(0) = 85 Β°C, and π = 25Β°C. πππ£
Tip: Remember to change the values to basic SI units! (for example 1 mm = 0.001 m).

Problem 5.
Study the data sheet for Pt100 tubular ceramic insert elements with tail wires. The aim is to estimate the thermal rate π for this sensor and draw the time response curve when it is placed from the room temperature (π = 22 Β°C) to hot water (π =
 100 Β°πΆ).
0
πππ£
   capacity πΆπ = 740 π½ . πππΎ
ππ3
T (degC)
??? ?
   Figure: Tubular ceramic encased Pt100 elements. The aim is to estimate the time response curve of the sensors when it is placed into hot water.
Firstly, letβs assume that the sensor element is mostly made of ceramics. The density of fused silica ceramic material is about π = 2.2 π and the mass-specific heat
time (s)
  We also assume that we can neglect the platinum filament inside the sensor. In addition, for the thermal analysis calculations we donβt care about the leads (wires) coming out from the sensor.
Figure: Wire-wound PRT. The platinum filament is coiled around the ceramic insulator and covered with ceramic shield (see element types in resistance thermometers). For thermal analysis we simplify and assume that the sensor element is made only of ceramic material.
  - the total volume π
- the total mass π, and
- the outer surface area of the ceramic element.
Letβs assume that the heat transfer coefficient for an object in hot water is about h = 1000 π .
Estimate
   π2πΎ
Based on all these calculations
- Estimate the thermal rate for the sensor.
- Draw the time response curve for this sensor.
- Based on the curve what is the sensorβs temperature at π‘ = 10.0 π .

Problem 6.
The time response of the temperature sensor can be modeled with a series RC-
- voltage π simulates the changes in the temperature of the external environment ππ
 circuit (see the figure) with a circuit simulator, where
- R and C models the thermal properties of the sensors, and
- voltage π models the temperature change of the sensor π.
π
 If the π is replaced with a signal step voltage source (Group: Sources, Family:
Figure: Series RC-circuit.
ππ
level voltages.
Figure: The settings for the STEP_VOLTAGE source. This component can be found from Sources > SIGNAL_VOLTAGE_SOURCES.
Build and simulate a series RC-circuit that models the time response of Pt100 sensors, when it is suddenly placed into boiling water (π = 22 Β°C , π = 100Β°C).
SIGNAL_VOLTAGE_SOURCES, Component: STEP_VOLTAGE), then the initial temperature π(0) and the final temperature π can be modeled as initial and final
- If π = 1.0 πΞ©, what the value of C should be, in order that the time constant is same as in previous problem?
πππ£
 0 πππ£
 - Verify that the output voltage is the same as the temperature in previous problem atπ‘ = 10.0π .
Tip 1: Thermal rate π and time constants π are reciprocals, e.g. π = 1/π.
Tip 2: You need to run transient analysis with start time 0 and find a suitable end time. To find a good value for it study transient analysis results graph.
