# ml-volcano
A Machine Learning project to predict time to erupt and amplitude of volcanoes
## Motivation
Volcanic eruptions pose significant risks to both human life and infrastructure. Early and accurate prediction of volcanic eruptions can enable timely evacuation and mitigation measures, potentially saving lives and minimizing damage. Machine learning techniques have shown promise in various domains, including regression tasks, and can potentially aid in forecasting volcanic eruptions.



## Introduction
Obtaining sensor readings from volcanic eruptions poses a significant challenge due to the limited number of active volcanoes worldwide and the infrequency of their eruptions. However, a collaboration between researchers at NVIDIA and NTU Singapore has yielded a promising solution. They have developed a mathematical model capable of simulating volcanic eruptions, enabling the generation of synthetic sensor readings. This innovative approach addresses the scarcity of real-world data by providing a reliable means of studying volcanic activity and its associated phenomena.

The synthetically generated dataset is a collection of diverse volcanoes. By altering the parameters of the mathematical model, synthetic observations are generated for each volcano. These parameters include Poisson's ratio (v), atmospheric pressure (Patm), gravity (g), radial distance tilt station (r), Sheer modulus (G), Magma density (rho), Magma viscosity (mu), conduit radius (rc), gas mass (M), standard deviation (sigma), tilt angle at eruption (tilt_erupt), and sensor values preceding the eruption event. 

The goal is to evaluate regression techniques' suitability for anticipating and comprehending volcanic phenomena using the synthetically generated dataset. The objective is to determine the effectiveness of these techniques in improving the understanding and predictive capabilities related to volcanic activities.



# Problem Statement
The problem at hand entails analyzing a sequence of sensor readings taken at consecutive time steps to address two distinct tasks related to volcanic eruptions. Firstly, the aim is to devise an effective approach that accurately estimates the remaining time units until eruption for a given observation. This observation can have sensor readings of varying lengths. By leveraging the information within the sensor data, the objective is to provide timely predictions for the impending eruption, enabling proactive measures to be taken to ensure the safety of affected areas and populations


The second task involves estimating the magnitude of the impending volcanic eruption. Utilizing the provided observation, the goal is to develop a methodology that can estimate the severity and intensity of the eruption event. Despite the absence of the eruption magnitude in the observations, it is possible to estimate the tilt erupt value, which represents the last sensor reading corresponding to the moment of eruption. This particular value exhibits a strong correlation with the magnitude of the eruption. By estimating the tilt erupt value, we can obtain a reliable estimation of the eruption's impact. The obtained estimation is crucial for emergency management and response planning, allowing authorities to allocate appropriate resources and implement necessary measures to mitigate the potential impacts of the volcanic eruption on surrounding areas.



