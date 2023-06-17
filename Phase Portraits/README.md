# Phase Portraits of Systems of ODE
Phase portraits are a way to visualize ODEs. The phase portrait tells in what direction a particle will move given its current state.

Fixed Points - These are the points which do not change with time. For example, for ODE $\dot{x} = \lambda x$, if $x = 0$, then the position will never change. Fixed points can be stable or unstable which can be determined using eigen values. Now eigen vectors are the directions where the ODEs are decoupled. So we use eigen vectors as the directions and check the stability and unstability along those directions.

The following discussion is based on 2x2 matrix as an example.

* Positive Eigen Values - When all the eigen values are positive then we get unstability in all the directions. In this type of system, we get a $\textbf{unstable source}$. It is called so because if the particle at the fixed point is perturbed a bit, it will flow away.

* Negative Eigen Values - When all the eigen values are negative then we get stability in all the directions. In this type of system, we get a $\textbf{stable sink}$. It is called so because if a particle at the fixed point is perturbed a bit, it will come down to the fixed point automatically.

* Saddle Point - When one eigen value is negative and one is positive, then the fixed point is called saddle point. It is called so, because in one direction the system is stable and in another direction, the system is unstable. So if particle is perturbed along one direction then it will return towards the point and if perturbed along the other direction, then it will flow away from the point.

* Complex eigen values - When the eigen values complex then we see oscillations because of the sin and cos terms. If the eigen values are purely complex, then phase portraits are concentric circles. This means that the particle will oscillate eternally. If there is a real part in the eigen value then there is some exponential growth or decay. So we will see an outward or inward spiral. This fixed point is called $\textbf{center fixed point}$. This is stable but is called marginally/neutrally stable.

Note - 
* As long as one direction is unstable, the system is called unstable. 
* Most real world systems are non-linear. So we observe the system near the fixed points. When we zoom into the fixed point then the system becomes linear around the fixed point.