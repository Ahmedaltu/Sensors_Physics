Assignment 6 – Thermal time response Sensor Physics 2022
Sakari Lukkarinen & Saana Vallius Metropolia University of Applied Sciences Instructions
First solve either problem 1 (easier) OR problem 2 (harder).
Then solve all the rest of the problems (3-5). Problem 1. (Easier)
Use pen and paper and verify by differentiation that 𝑇=𝑇 +(𝑇−𝑇 )⋅𝑒
where T’ is temperature’s rate of change.
Use the following numerical values for the solution:
Use paper and pen and verify by separation of variables that
Use the following numerical values for the solution:
𝑇(0) = 20 °C, 𝑇 = 100 °C, and 𝑟 = 0.10 1.
Tip 1: The first step in separation is the following: 𝑑𝑇 = −𝑟 ⋅ 𝑑𝑡 (𝑇−𝑇 )
𝑒𝑛𝑣
Tip 2: Review Engineering Mathematics lecture notes.
𝑒𝑛𝑣 0 𝑒𝑛𝑣
−𝑟𝑡
 is a solution for the Newton’s law of cooling differential equation
′
𝑇=−𝑟(𝑇−𝑇 )
𝑇(0)=20°C,𝑇 =100°C,and𝑟=0.10 1 𝑒𝑛𝑣 𝑠
Tip 1: First replace all symbols with their numerical values in the equations. Then differentiate the solution for 𝑇, substitute 𝑇’ and 𝑇 into the Newton’s law of cooling differential equation and simplify it to see that both sides are equal.
Tip 2: Review Engineering Mathematics lecture notes. Problem 2. (Harder)
𝑇(𝑡)=𝑇 +(𝑇−𝑇 )⋅𝑒 𝑒𝑛𝑣 0 𝑒𝑛𝑣
𝑑𝑡
𝑒𝑛𝑣
𝑒𝑛𝑣
𝑒𝑛𝑣 𝑠
−𝑟𝑡
 is a solution for the Newton’s law of cooling differential equation
𝑑𝑇=−𝑟(𝑇−𝑇 )
 
Problem 3.
Sketchagraphofthesolution𝑇(𝑡)=𝑇 +(𝑇 −𝑇 )⋅𝑒 usingthegiven
Use pen and paper, Scientific Python, Excel, or any other tool you are familiar with to calculate the values and plot the graph.
Problem 4.
In thermal systems, the thermal rate 𝑟 can be expressed as
𝑒𝑛𝑣 0 𝑒𝑛𝑣
−𝑟𝑡
numerical values 𝑇(0) = 20 °C, 𝑇 = 100 °C, and 𝑟 = 0.10 1 in the range 𝑡 = 0 ... 60 𝑠 𝑒𝑛𝑣 𝑠
𝑟= h𝐴,where 𝐶𝑡𝑜𝑡
- h is the heat transfer coefficient between the system and the environment,
- 𝐴 is the surface area of the system, and
- 𝐶𝑡𝑜𝑡 is the total heat capacity of the system.
 The total heat capacity 𝐶𝑡𝑜𝑡 can be represented by its mass-specific heat capacity 𝐶𝑝 multiplied by its mass 𝑚 𝐶𝑡𝑜𝑡 = 𝐶𝑝 ⋅ 𝑚
 So, the thermal rate 𝑟 becomes to
Find the thermal rate, if the system has the following properties
h=150 𝑊 ,𝐴=590𝑚𝑚2,𝑚=0.76𝑔,and𝐶 =730 𝐽 𝑚2𝐾 𝑝 𝑘𝑔𝐾
𝑟= h𝐴 𝐶𝑝𝑚
Sketch a graph of the temperature for the system following Newton’s law of cooling (problems 1-3) for
𝑡 = 0 ... 30 𝑠, 𝑇(0) = 85 °C, and 𝑇 = 25°C. 𝑒𝑛𝑣
Tip: Remember to change the values to basic SI units! (for example 1 mm = 0.001 m).

Problem 5.
Study the data sheet for Pt100 tubular ceramic insert elements with tail wires. The aim is to estimate the thermal rate 𝑟 for this sensor and draw the time response curve when it is placed from the room temperature (𝑇 = 22 °C) to hot water (𝑇 =
 100 °𝐶).
0
𝑒𝑛𝑣
   capacity 𝐶𝑝 = 740 𝐽 . 𝑘𝑔𝐾
𝑐𝑚3
T (degC)
??? ?
   Figure: Tubular ceramic encased Pt100 elements. The aim is to estimate the time response curve of the sensors when it is placed into hot water.
Firstly, let’s assume that the sensor element is mostly made of ceramics. The density of fused silica ceramic material is about 𝜌 = 2.2 𝑔 and the mass-specific heat
time (s)
  We also assume that we can neglect the platinum filament inside the sensor. In addition, for the thermal analysis calculations we don’t care about the leads (wires) coming out from the sensor.
Figure: Wire-wound PRT. The platinum filament is coiled around the ceramic insulator and covered with ceramic shield (see element types in resistance thermometers). For thermal analysis we simplify and assume that the sensor element is made only of ceramic material.
  - the total volume 𝑉
- the total mass 𝑚, and
- the outer surface area of the ceramic element.
Let’s assume that the heat transfer coefficient for an object in hot water is about h = 1000 𝑊 .
Estimate
   𝑚2𝐾
Based on all these calculations
- Estimate the thermal rate for the sensor.
- Draw the time response curve for this sensor.
- Based on the curve what is the sensor’s temperature at 𝑡 = 10.0 𝑠.

Problem 6.
The time response of the temperature sensor can be modeled with a series RC-
- voltage 𝑉 simulates the changes in the temperature of the external environment 𝑖𝑛
 circuit (see the figure) with a circuit simulator, where
- R and C models the thermal properties of the sensors, and
- voltage 𝑉 models the temperature change of the sensor 𝑇.
𝑐
 If the 𝑉 is replaced with a signal step voltage source (Group: Sources, Family:
Figure: Series RC-circuit.
𝑖𝑛
level voltages.
Figure: The settings for the STEP_VOLTAGE source. This component can be found from Sources > SIGNAL_VOLTAGE_SOURCES.
Build and simulate a series RC-circuit that models the time response of Pt100 sensors, when it is suddenly placed into boiling water (𝑇 = 22 °C , 𝑇 = 100°C).
SIGNAL_VOLTAGE_SOURCES, Component: STEP_VOLTAGE), then the initial temperature 𝑇(0) and the final temperature 𝑇 can be modeled as initial and final
- If 𝑅 = 1.0 𝑘Ω, what the value of C should be, in order that the time constant is same as in previous problem?
𝑒𝑛𝑣
 0 𝑒𝑛𝑣
 - Verify that the output voltage is the same as the temperature in previous problem at𝑡 = 10.0𝑠.
Tip 1: Thermal rate 𝑟 and time constants 𝜏 are reciprocals, e.g. 𝜏 = 1/𝑟.
Tip 2: You need to run transient analysis with start time 0 and find a suitable end time. To find a good value for it study transient analysis results graph.
