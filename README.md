# Solar charge controller with Maximum Power Point Tracking (MPPT)
There are naturally power losses that take place when the solar panel is directly connected to load/battery without matching its operating characteristics under varying solar isolation and operating temperature.
To develop an efficient, simple, durable, adaptable setup for power harvesting solar charge controller with Maximum Power Point Tracker(MPPT) is needed.


Maximum Power Point Tracker(MPPT), a power electronic device which significantly increases the Photovoltaic system efficiency.
By using MPPT, the system operates at Maximum Power Point(MPP) and produces its maximum power output.
MPPT maximizes the array efficiency, thereby reducing the overall system cost.

![image](https://user-images.githubusercontent.com/87081314/126138731-f442574f-d273-494b-878a-a72741259489.png)

## PV Cell Decription
 - PV array 30V, 230 Watt,single array
 - DC-DC buck-boost converter
 - 12V, 100ah battery
 - MPPT's algorithm:P&O and IC.

![image](https://user-images.githubusercontent.com/87081314/126138977-a428286b-4f05-454a-bf54-ff2ea2233f63.png)


### MPPT Techniques

**Perturb and Observe Algorithm**

![image](https://user-images.githubusercontent.com/87081314/126139403-4066688c-8876-4f98-a13c-baec8a4ce34b.png)
![image](https://user-images.githubusercontent.com/87081314/126139475-568845b8-bf68-4bad-8cd7-2dc04b8fa3b3.png)

P&O is the most widely used algorithm due to the simplicity of implementation practically.
In this method, PV characteristics of PV cell is used.
The main advantage of P&O algorithm are simple structure and ease of implementation, with both stand alone and grid connected systems.
MPP tracking efficiency is good but with unstable operating point.

**Incremental Conductance**

![image](https://user-images.githubusercontent.com/87081314/126140177-4bac4db7-e43f-4aa6-879a-ed7a70cb841f.png)
![image](https://user-images.githubusercontent.com/87081314/126140232-ffa454b4-0394-4386-984d-518f165532f6.png)

In literature, Incremental conductance method was determined to operate with more efficiency under randomly generated conditions.
Oscillation problem of P&O algorithm around MPP is eliminated.
The cost is high due to requirements of high sampling compliance and speed control as a result of complex structure.

**DC to DC converter - BuckBoost**

Buck-Boost converter is basically one type of DC-DC converter which has output voltage either greater or less than the input voltage magnitude.
There are two types of topologies – Inverting and Non-Inverting.
A Buck converter step down voltage from its input to its output load.
A Boost converter step up voltage from its input to its output load.
It offers high efficiency with low cost and components.

**Components**
DC voltage source
MOSFETs
Inductor
Diode
Capacitor

![image](https://user-images.githubusercontent.com/87081314/126140816-d375dbf4-d95f-457b-8590-b79140e4af79.png)

#### **System requirements**

Simulation Software: **MATLAB**
Version: **R2017** and above can be used  

The project focuses on the MATLAB/Simulink model for continuous monitoring of maximum output of a PV panel, conducted a comparative analysis of buck-boost converter with two algorithms **"Perturb and Observe"** and **"Incremental conductance"**.



##### **How to run?**

Open mpptbuckboostpando.mdl, mpptbuckboostIncrementalConductance.slx file with MATLAB/Simulink.
Set the configuration parameters as Type:Fixed step,Solver:Discrete 
Run the simulation
Click on the scope to have a graphical view.

###### **Working of simulation**

The PV panel measure gives the PV voltage, the PV current that is  introduced in the MPPT function that gives the necessary increase/decrease of the duty cycle for the MOSFET switching in the dc-dc converter.
As the irradiance decreases, the PV power falls  that  is visible as a drop in the current on the battery side.

###### **Contributions**
- Asma Ul Husna
- Dharani
- Madhumitha

**Mentored by**:Kiran Kumar

















