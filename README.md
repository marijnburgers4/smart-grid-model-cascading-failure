

## **1. Introduction**:
For my Master Thesis at TU Delft (faculty of Technology, Policy & Management, programme: Complex Systems Engineering & Management) I analysed cascading failures initialised in the communication network. I developed an interdependent communication network and power grid (a smart grid). The communication network is created using NetworkX library and pandapower is used to create the power grid.

## **2. The model**:
   A brief overview of the steps of the smart grid model failure simulation:

   ![Grid Diagram](https://github.com/marijnburgers4/smart-grid-model-cascading-failure/blob/main/steps%20in%20the%20model%20simulation.png?raw=true)

   
A communication network is generated using Python and network theory. This communication network is coupled with a one-to-one interdependency with a power grid. To give the power grid electrical characteristics, we use Pandapower's IEEE 118-bus test system. A failure of a communication network component leads to a failure of the power grid component and vice versa. We simulate failure scenarios by increasingly failing communication network nodes based on random selection and targeted attacks (degree, betweenness, and closeness centrality). This is applied to two types of communication networks: a double-star and a mesh network. Additionally, we incorporate two different model behaviours: one that includes failure propagation in the communication network (using a simple diffusion model to simulate, for example, virus spread) and one that does not. How the failure propagation can be activated or deactivated is explained in the notebook code in section 'The Simulation'
## **3. Installation**:
   The model is created in a Juypter Notebook vers. 7.0.8,  We used Python vers. 3.9.18 through Anaconda.

## **4. Usage**:
When opening the notebook file, there is short description on how to run each cell (which sequence)

