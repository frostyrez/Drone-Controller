# Drone-Controller
For my Masters Final Year Project at the University of Bath, I obtained a 75% (First) for the design of a robust non-linear Multiple-MPC-based controller to achieve the goal and title of the project, “Predictive Control of Autonomous Quadcopters”. See Report for a full breakdown, or below for a brief outline of the work carried out.

This began with the derivation of a mathematical model of a standard quadcopter, comprising 16 states, 3 coordinate frames, and the equations relating them. State derivatives, forces and torques were then established, with the physical properties of the DJI F450 representing the quadcopter. 

![image](https://github.com/user-attachments/assets/f5bd3644-e85d-4bca-8f44-1a7645da57b2)

Eventually, this model was ported to Simulink, with various linear closed-loop controllers connected to it, like PID, LQR, and MPC. 

![image](https://github.com/user-attachments/assets/7efa6953-dc44-4241-8f6c-e1bb1553fab8)

The gains in the controllers were then individually tuned to optimise performance. 

![image](https://github.com/user-attachments/assets/4b1e1eb3-6200-4046-833a-18bcc97757e9)

These controllers were then evaluated against a fully-tuned linear MPC, which leverages control and prediction horizons to optimize its inputs. This results in even better performance than LQR, albeit at the cost of increased computational time.
