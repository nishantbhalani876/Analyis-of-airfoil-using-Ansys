## CFD Analysis of Airfoil at 0 Degree Angle of Attack (Axisymmetric Model)

This report details the computational fluid dynamics (CFD) analysis of an airfoil using an axisymmetric modeling approach within Ansys Fluent. The primary objective was to determine the lift and drag coefficients at a 0-degree angle of attack and compare these results against experimental data to quantify the error.

### Methodology

The CFD simulation was performed using Ansys Fluent, employing an axisymmetric model to represent the airfoil. This approach simplifies the 3D geometry into a 2D cross-section, significantly reducing computational cost while providing a reasonable approximation for certain flow conditions, particularly at zero angle of attack where 3D effects might be less dominant.

* **Software:** Ansys Fluent
* **Modeling Approach:** Axisymmetric
* **Angle of Attack ($\alpha$):** 0 degrees

### Boundry Condition 
* **Inlet** Velocity : 45.6 m/s
* turbulence Intensity : 5%
* **Outlet Pressure :** 0 gauge pressure
* **Airfoil Wall Boundary Condition** : No Slip Wall

### Meshing 
* No. of Nodes : 509638
<img width="903" height="633" alt="Airfoil Mesh" src="https://github.com/user-attachments/assets/d7368e23-4b0b-4065-8082-07acd42125b1" />

### Results and Discussion

The CFD simulation yielded the following lift and drag coefficients:

* **Calculated Lift Coefficient ($C_L$):** $0.26108561$
* **Calculated Drag Coefficient ($C_D$):** $0.0075254815$

These numerical results were then compared against available experimental data for the same airfoil and operating conditions:

* **Experimental Lift Coefficient ($C_L$):** $0.25$
* **Experimental Drag Coefficient ($C_D$):** $0.0065$

Velocity Contour : 

### Error Analysis

The percentage error between the calculated and experimental coefficients was determined as follows:

* **Percentage Error in Lift Coefficient:** $4.4$%
* **Percentage Error in Drag Coefficient:** $15.69$%

Expermintal values at different Angle of Attacks<img width="1191" height="879" alt="image" src="https://github.com/user-attachments/assets/806aefe4-69b0-4792-b6ec-ce2ded6c96f9" />


The discrepancies between the CFD results and experimental data can be attributed to several factors, including:

* **Assumptions of Axisymmetric Model:** While computationally efficient, the axisymmetric simplification may not fully capture all three-dimensional flow phenomena that could be present even at 0 degrees angle of attack.
* **Turbulence Model Limitations:** The choice of turbulence model can significantly impact the accuracy of CFD predictions, especially in regions of flow separation or complex boundary layers.
* **Mesh Resolution:** The quality and density of the computational mesh can influence the accuracy of the solution.
* **Experimental Uncertainties:** Experimental data inherently contains measurement uncertainties that contribute to the overall discrepancy.
