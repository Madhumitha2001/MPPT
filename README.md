# Solar charge controller with Maximum Power Point Tracking (MPPT)
There are naturally power losses that take place when the solar panel is directly connected to load/battery without matching its operating characteristics under varying solar isolation and operating temperature.
To develop an efficient, simple, durable, adaptable setup for power harvesting solar charge controller with Maximum Power Point Tracker(MPPT) is needed.


Maximum Power Point Tracker(MPPT), a power electronic device which significantly increases the Photovoltaic system efficiency.
By using MPPT, the system operates at Maximum Power Point(MPP) and produces its maximum power output.
MPPT maximizes the array efficiency, thereby reducing the overall system cost.

![image](https://user-images.githubusercontent.com/87081314/126138731-f442574f-d273-494b-878a-a72741259489.png)

Photovoltaic cell - Characteristics

![image](https://user-images.githubusercontent.com/87081314/126138977-a428286b-4f05-454a-bf54-ff2ea2233f63.png)


MPPT Techniques

Perturb and Observe Algorithm

![image](https://user-images.githubusercontent.com/87081314/126139403-4066688c-8876-4f98-a13c-baec8a4ce34b.png)
![image](https://user-images.githubusercontent.com/87081314/126139475-568845b8-bf68-4bad-8cd7-2dc04b8fa3b3.png)

P&O is the most widely used algorithm due to the simplicity of implementation practically.
In this method, PV characteristics of PV cell is used.
The main advantage of P&O algorithm are simple structure and ease of implementation, with both stand alone and grid connected systems.
MPP tracking efficiency is good but with unstable operating point.

Incremental Conductance

![image](https://user-images.githubusercontent.com/87081314/126140177-4bac4db7-e43f-4aa6-879a-ed7a70cb841f.png)
![image](https://user-images.githubusercontent.com/87081314/126140232-ffa454b4-0394-4386-984d-518f165532f6.png)

In literature, Incremental conductance method was determined to operate with more efficiency under randomly generated conditions.
Oscillation problem of P&O algorithm around MPP is eliminated.
The cost is high due to requirements of high sampling compliance and speed control as a result of complex structure.

DC to DC converter - BuckBoost

Buck-Boost converter is basically one type of DC-DC converter which has output voltage either greater or less than the input voltage magnitude.
There are two types of topologies – Inverting and Non-Inverting.
A Buck converter step down voltage from its input to its output load.
A Boost converter step up voltage from its input to its output load.
It offers high efficiency with low cost and components.

BuckBoost converter

COMPONENTS

DC voltage source,
MOSFETs,
Inductor,
Diode,
Capacitor,

![image](https://user-images.githubusercontent.com/87081314/126140816-d375dbf4-d95f-457b-8590-b79140e4af79.png)

Simulation

Software : Matlab,
 Version    : 2021a

MPPT using P&O algorithm

![image](https://user-images.githubusercontent.com/87081314/126141565-562727ec-4eb1-468f-9177-ea6e87931c11.png)

Results

![image](https://user-images.githubusercontent.com/87081314/126141650-be224415-c3f1-47cd-ad21-44980aca2fdf.png)

MPPT using Incremental Conductance

![image](https://user-images.githubusercontent.com/87081314/126142058-6d2f3383-a963-4e5a-80e3-e3e742c47142.png)

Results

![image](https://user-images.githubusercontent.com/87081314/126142117-8e573a07-011a-4756-b160-05ab997ff3d0.png)

















