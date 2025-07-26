## Drone Payload Simulation - MathWorks Internship Group 4 Project Submission
### Group 4
- Javier Mazorra
- Eleen Gregoryona (she/her)
- Skyler Andrade Flores
- Saige Sloan (they/them)
___
### Project Description
The purpose of this project is to optimize drone delivery by establishing a design that can carry heavier packages. Our objective is to maximize package weight and keep the overall drone/structure lightweight, without compromising stability or control.

We applied various engineering concepts including:
- CAD modeling (SolidWorks)
- MATLAB/Simulink simulation
- Truss analysis
- Engineering design tradeoffs

The 3D model and simulation environment serve as a foundation for future work on drone mechanics and control systems for autonomous delivery.
___
### Project Improvements/Limitations
Our SolidWorks model showcases the design of a sturdy drone and implements a truss on each leg to reduce weight load. When running our simulation on Simulink, we can observe the movement of the propellers, however, there is unfortunately no movement or path for the drone to travel. Acknowledging this, there should be improvements made to the Simulink network, as the lack of movement is the main issue when running the simulation.
___
### Interacting / Using this Project
#### Requirements
- MATLAB R2023b or later
- Simulink
- Simscape Multibody
- Simscape Multibody Link (for importing from SolidWorks)

### Running the Model
1. **Clone the repository:**
   ```bash
   git clone https://github.com/seasaltsaige/drone-structure-design-and-analysis-group-4
   cd drone-payload-sim
   ```
2. **Open Simulink Model:**

   ```bash
   open('Prototype_3.slx')
   ```
   Alternatively, open Simulink through Matlab, then open the .slx file through the explorer.
3. **Run the simulation:**

   The model currently spins the propellers at a fixed rate, but does not yet have any lift or motion.
___
### File Structure
```bash
┌ drone-structure-design-and-analysis-group-4
├── drone-model
│   ├── Drone fin cap_Default_sldprt.STEP
│   ├── Drone Legs_Default_sldprt.STEP
│   ├── Drone motor_Default_sldprt.STEP
│   ├── DRONE-FRAME-LIGHT-CUT_Default_sldprt.STEP
│   ├── package holder_Default_sldprt.STEP
│   └── Propellor_Default_sldprt.STEP
├── media
│   ├── Drone_Bottom.png
│   ├── Drone_Side.png
│   ├── Drone_Still.png
│   ├── Prototype_3.avi
│   ├── Simulink_Bottom.png
│   ├── Simulink_Top.png
│   └── Simulink.png
├── LICENSE
├── Prototype_3_DataFile.m
├── Prototype_3.slx
├── Prototype_3.xml
└── README.md
```
- **drone-model/**: contains the generated step files created and exported in SolidWorks.
- **media/**: contains screenshots and videos of the drone in Simulink, along with the corresponding Simulink block diagram of system setup.
- **LICENSE**: open source license required for the MathWorks internship submission
- **Prototype_3_DataFile.m**: generated Simscape Multibody data file for the drone body.
- **Prototype_3.slx**: Simulink model file
- **Prototype_3.xml**: linking file which describes positioning and transforms of all related drone parts.
___
### Individual Contributions
Starting off, each student performed research on drone design and delivery in regards to external weight and load paths. From there, two students designed the drone on SolidWorks and experimented with different prototypes, to ensure the next was improved through a reduction in material. The other two students then worked through Simulink to generate a system that could closely emulate drone flight and understand more of the mechanics behind getting a simulation to run. Then once the SolidWorks files were converted to be used in Simulink, we created a new system that could implement each component of the drone.

## Acknowledgements
This project was made during and for the MathWorks Summer 2025 Internship, for Group 4.

We are grateful to the MathWorks team and mentors for their guidance and support with issues that arise during the duration of the program. Additionally, we are grateful for the opportunity to engage in applied simulation and modeling challenge. 