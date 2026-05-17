DIGITAL TWIN-BASED TRANSFORMER OVERLOAD PREVENTION SYSTEM FOR EV INTEGRATION 

A Digital Twin-based & adaptive EV charging system that monitors transformer load in real time and dynamically controls charging to prevent overload using MATLAB/Simulink.

The **Digital Twin Based Adaptive EV Charging System for Transformer Overload Prevention** is an intelligent solution designed to optimize electric vehicle (EV) charging while ensuring the safe operation of distribution transformers. The system leverages digital twin technology to create a real-time virtual model of a physical transformer, enabling continuous monitoring and predictive analysis.

In this project, real-time parameters such as load demand, voltage, and current are monitored and fed into a simulation model developed in MATLAB/Simulink. The digital twin replicates the behavior of the transformer under varying load conditions and evaluates its performance dynamically.

Based on this analysis, the system implements an adaptive EV charging strategy that regulates charging power according to transformer loading conditions. When the transformer approaches critical limits, the charging rate is automatically adjusted to prevent overload, thereby enhancing system reliability and extending equipment lifespan.

Additionally, the system can incorporate basic machine learning techniques, such as regression-based prediction, to forecast load trends and improve decision-making accuracy. This enables proactive control rather than reactive responses.

Overall, the proposed system demonstrates a smart grid approach by integrating digital twin technology, adaptive control, and EV charging infrastructure, contributing to efficient energy management and sustainable transportation.

** Objectives **

1 Monitor transformer load in real time
2 Prevent transformer overload during EV charging
3 Implement adaptive charging control
4 Improve power system reliability

 ** Technologies Used **

1 MATLAB / Simulink
2 Digital Twin Modeling
3 Basic Machine Learning (Regression)
4 Power System Analysis

 MATLAB/Simulink Model

![MATLAB Model](MATLAB_MODEL.png)

This is my developed MATLAB/Simulink model for the Digital Twin Based Adaptive EV Charging System. The model represents the complete system including:

- Three-phase grid and transformer setup  
- Voltage and current measurement blocks  
- Transformer loading calculation  
- EV charging load integration  
- Adaptive control mechanism  
- Digital twin-based prediction and decision system  

The model continuously monitors transformer loading conditions and dynamically adjusts EV charging power to prevent overload, ensuring safe and efficient operation of the power system.

** Working Principle **

The system creates a digital twin of the transformer using MATLAB/Simulink. Real-time load data is analyzed and compared with the simulated model. Based on transformer loading conditions, the EV charging rate is dynamically adjusted to prevent overload and ensure safe operation.

** Results **

1. Normal Loading Condition
![Normal Load](RES_1_Normal_Loading.png)
Under normal operating conditions, the transformer supplies both domestic load and EV charging load within its rated capacity. The total transformer loading remains below the predefined safe operating threshold of 80%.

In this condition:

The three-phase voltage and current waveforms remain balanced and sinusoidal.
No overload condition occurs in the system.
Transformer loading stays stable around the normal operating region.
Since the loading percentage does not exceed the threshold limit, the controller remains inactive.
The Digital Twin continuously monitors system behavior and compares actual loading with predicted loading for real-time supervision.

The simulation result confirms that the transformer operates safely and efficiently under standard loading conditions without requiring any control action.

2. Overload Condition (Without Control)
![Overload Without Control](RES_2_OverLoaded(NO_controller).png)
This figure shows the transformer operating under overload conditions without any control action applied.

As EV charging demand increases, the total transformer loading crosses the predefined safe limit of 80%. The increase in load causes the transformer current to rise while the system continues operating in an overloaded state.

From the graph, it can be observed that the transformer loading percentage remains above the safe operating threshold. Since no controller is present, the EV load continues to consume high power without any regulation or load reduction.

Operating continuously under this condition can negatively affect transformer performance by:

increasing thermal stress,
overheating transformer components,
reducing insulation life, and
decreasing overall system reliability.

Although the Digital Twin model is able to detect and monitor the overload condition in real time, no corrective action is taken in this case. This demonstrates the importance of implementing an intelligent control system to regulate EV charging demand and maintain transformer loading within safe operating limits.
In this scenario, the transformer experiences overload due to uncontrolled EV charging demand.

3. Overload Condition (With Adaptive Control)
![Overload With Control](RES_3_OverLoaded(WITH_Controller).png)
This figure shows the transformer behavior under overload conditions when the proposed control system is enabled.

Initially, the transformer loading exceeds the predefined safe operating limit of 80% due to increased EV charging demand. Once the overload condition is detected, the controller automatically reduces the EV charging load to protect the transformer from operating in an unsafe region.

From the graph, it can be observed that the transformer loading percentage initially rises above the threshold limit. After controller activation, the loading gradually decreases and stabilizes below the safe operating limit.

The reduction in current magnitude after controller action clearly indicates successful load regulation by the system.

This controlled operation helps in:

preventing transformer overheating,
reducing electrical stress,
improving system reliability, and
maintaining stable transformer operation during high EV demand conditions.

The Digital Twin continuously monitors transformer loading and supports the controller by analyzing real-time operating conditions and predicted load behavior. The simulation result demonstrates the effectiveness of intelligent EV load management in maintaining transformer loading within safe limits.

The adaptive EV charging system reduces the charging load to prevent transformer overload.

4. Digital Twin Performance
![Digital Twin Performance](RES_4_DIGITAL_TWIN_PERFORMANCE.jpeg)
This figure shows the performance of the proposed Digital Twin model by comparing the actual transformer loading with the predicted loading generated by the system.

The upper graph represents the overall transformer loading variation during different operating conditions, including overload and controlled regions. It can be observed that the predicted load closely follows the actual transformer load throughout the simulation.

The lower graph provides a zoomed-in view of the comparison, clearly showing the close alignment between actual and predicted loading values. The small deviation between the two curves indicates that the prediction model is able to estimate transformer loading with good accuracy.

The Digital Twin continuously monitors system behavior and predicts loading trends in real time using a basic Linear Regression-based approach. This prediction capability helps the controller make faster and more effective decisions during overload conditions.

The result demonstrates that the proposed Digital Twin model can:

monitor transformer loading effectively,
estimate future loading conditions,
support intelligent EV load control, and
improve overall reliability of the power distribution system.

This validates the effectiveness of integrating Digital Twin concepts with AI-assisted load prediction for transformer overload prevention in EV charging applications.

This result demonstrates how the digital twin model effectively monitors and controls the system for safe operation.
1 Reduced transformer overload conditions
2 Improved charging efficiency
3 Better load management


This project demonstrated a Digital Twin-Based Transformer Overload Prevention System for EV integration using MATLAB/Simulink. The system continuously monitored transformer loading and detected overload conditions caused by increased EV charging demand. A control system was implemented to reduce EV load whenever transformer loading exceeded the safe operating limit of 80%. The simulation results confirmed stable and safe transformer operation under controlled conditions. The Digital Twin model also showed good agreement between predicted and actual loading values, supporting intelligent load management in modern power systems.

⚙️ Key Points
Top Graph: Three-phase voltage waveforms
Middle Graph: Three-phase current waveforms
Bottom Graph: Transformer loading percentage compared with the safe loading threshold (80%)
