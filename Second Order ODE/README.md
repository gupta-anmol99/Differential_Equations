# Second Order Systems
To understand second order systems, damped harmonic oscillators can be used. 

Damped Harmonic Oscillators can be defined by equation -

$$m\ddot{x} = -kx -d\dot{x}$$

Here, $m = mass$, $k = spring constant$, $x = position$ & $d = damping coefficient$.

Now we will define $\zeta = \frac{{d}}{{2\sqrt{mk}}}$ & $\omega^2 = \frac{k}{m}$

Using this, the equation converts into -
$$\ddot{x} + 2\omega\zeta\dot{x} + \omega^2x$$

In this equation, $\omega$ is called natural frequency and $\zeta$ is called damping ratio. The system is called underdamped when $\zeta < 1$, the system is called overdamped when $\zeta > 1$ and the system is called critically damped $\zeta = 1$.

Now, to solve a linear ODE, we guess the solution to be of the form $x = e^{\lambda t}$. This gives us $\dot{x} = \lambda e^{\lambda t}$ and  $\ddot{x} = \lambda^2 e^{\lambda t}$.

Plug these values in the equation. We get - 
$$e^{\lambda t}(\lambda^2 + 2\omega\zeta\lambda + \omega^2) = 0$$

Since $e^{\lambda t}$ cannot be zero, we equate the quadratic equation to be zero. Solving this, we get $\lambda_{1,2} = \frac{{-2\omega\zeta \pm \sqrt{(2\omega\zeta)^2 - 4\omega^2}}}{2}$.

Since the linear ODE follow superposition rule, the solution comes out to be - 

$$x(t) = c_1e^{\lambda_1t} + c_2e^{\lambda_2t}$$

## Solving as system of diffrential equations.
We can convert second order ODE into 2 first order coupled ODE. To do this, we introduce another variable $v$, where $v = \dot{x}$.

Now we can write the system of equations in the form - 
$$\frac{d}{dt}\left[x \atop v\right] = {\left\lbrack \matrix{0 & 1 \cr -\omega^2 & -2\omega\zeta} \right\rbrack}\left[x \atop v\right]$$.




