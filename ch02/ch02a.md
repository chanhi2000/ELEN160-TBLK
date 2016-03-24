# Chaos, Complexity and Self-Organization

## What is Chaos?
The practice of modeling physical systems using differential equations dates back to the 17th century, and the development of Newtonian mechanics. Over the past three hundred years, mathematical descriptions of this type have been successfully applied in a wide variety of disciplines, ranging from physics and engineering to economics and biology. Almost without ಆxception, the underlying equations allowed scientists to accurately predict the dynamics of such systems, and explain the observed experimental data. As a result, there was no reason to suspect that a purely determi uncertainties of any kind.

Systems where chaos has been observed are also described in terms of differential equations, which are simple and precisely defined as those of classical mechanics. And yet, it turns out that these systems possesses some very unusual properties, which cannot be anticipated from the structure of the mathematical models that govern their dynamics.

Perhaps the easiest way to describe these properties is to contrast chaos to the behavior of a classical system such as the pendulum shown in Fig. 2.1

![diagram of a pendulum](ch02/ch02-fig2-01.png)
###### Figure 2.1


A pendulum has all the characteristics that one would expect to see in a deterministic mechanical system. Its dynamics can be described by two simple first order differential equations, and its trajectory is completely predictable once we provide the initial angle and velocity (the so-called initial conditions). The typical behavior of a pendulum is illustrated in [Figs. 2.2](#figure-2-1-) and [2.3](), which show how the angle $$\theta(t)$$ and velocity $$\omega(t)$$ evolve over time. It is obvious that both variables exhibit a regular oscillatory pattern, and that the system stops moving after a sufficiently long time (ultimately settling down into an equilibrium state). We should also point out that these plots will not change in any meaningful way if the initial conditions are slightly altered. Such insensitivity to small variations ensures that repeated physical experiments with this system will always yield consistent results, although we can never perfectly replicate all the conditions.

In the analysis of dynamic systems such as a pendulum, it is common practice to supplement the graphs shown in [Figs. 2.2](#figure-2.1) and [2.3]() with a plot of the velocity $$\omega$$ as a function of angle $$\theta$$. If we were to do that, we would see that all solutions ultimately converge to the equilibrium point $$(\theta^e,\:\omega^e)=(0,\:0)$$, regardless of where they start from. In this case the equilibrium acts as a sort of “magnet” that “draws in" different trajectories, which is why we refer to it as an attractor. This property is illustrated in Fig. 2.4, where we show two different trajectories of a pendulum – one starting out from initial condition $$(\theta_0,\:\omega_0)=(1,\:1)$$, and the other from $$(\theta_0,\:\omega_0)=(-1,\:-1)$$. Both of them obviously converge to point $$(0,\:0)$$.


