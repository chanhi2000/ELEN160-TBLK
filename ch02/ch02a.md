## 2.1 What is Chaos?

The practice of modeling physical systems using differential equations dates back to the 17th century, and the development of Newtonian mechanics. Over the past three hundred years, mathematical descriptions of this type have been successfully applied in a wide variety of disciplines, ranging from physics and engineering to economics and biology. Almost without ಆxception, the underlying equations allowed scientists to accurately predict the dynamics of such systems, and explain the observed experimental data. As a result, there was no reason to suspect that a purely determi uncertainties of any kind.

Systems where chaos has been observed are also described in terms of differential equations, which are simple and precisely defined as those of classical mechanics. And yet, it turns out that these systems possesses some very unusual properties, which cannot be anticipated from the structure of the mathematical models that govern their dynamics.

Perhaps the easiest way to describe these properties is to contrast chaos to the behavior of a classical system such as the pendulum shown in __Fig. 2.1__

![fig2-01](ch02/ch02-fig2-01.png)
#### Fig. 2.1. Diagram of a pendulum.

A pendulum has all the characteristics that one would expect to see in a deterministic mechanical system. Its dynamics can be described by two simple first order differential equations, and its trajectory is completely predictable once we provide the initial angle and velocity (the so-called *initial conditions*). The typical behavior of a pendulum is illustrated in __Figs. 2.2__ and __2.3__, which show how the angle $$\theta(t)$$ and velocity $$\omega(t)$$ evolve over time. It is obvious that both variables exhibit a regular oscillatory pattern, and that the system stops moving after a sufficiently long time (ultimately settling down into an *equilibrium state*). We should also point out that these plots will *not* change in any meaningful way if the initial conditions are slightly altered. Such insensitivity to small variations ensures that repeated physical experiments with this system will always yield consistent results, although we can never perfectly replicate all the conditions.

In the analysis of dynamic systems such as a pendulum, it is common practice to supplement the graphs shown in __Figs. 2.2__ and __2.3__ with a plot of the velocity $$\omega$$ as a function of angle $$\theta$$. If we were to do that, we would see that all solutions ultimately converge to the equilibrium point $$(\theta^e,\:\omega^e)=(0,\:0)$$, regardless of where they start from. In this case the equilibrium acts as a sort of “magnet” that “draws in" different trajectories, which is why we refer to it as an attractor. This property is illustrated in Fig. 2.4, where we show two different trajectories of a pendulum – one starting out from initial condition $$(\theta_0,\:\omega_0)=(1,\:1)$$, and the other from $$(\theta_0,\:\omega_0)=(-1,\:-1)$$. Both of them obviously converge to point $$(0,\:0)$$.

![fig2-02](ch02/ch02-fig2-03.png)
#### Fig. 2.2 The angle of the pendulum

![fig2-03](ch02/ch02-fig2-04.png)
#### Fig. 2.3 The angular velocity of a pendulum

![fig2-04](ch02/ch02-fig2-04.png)
#### Fig. 2.4 Two Trajectories for a pendulum

There are, of course, many other physical systems in which equilibria act as attractors. Figure 2.5 (which represents a predator-prey model in theoretical biology) shows that in some cases there are actually several such equilibria, each one “drawing in" a different set of trajectories. Note that in this particular example some solutions diverge, and have nothing to do with the pair of attractors (these would be the two trajectories originating in the lower right-hand corner of the diagram).

What can we conclude from this brief discussion? If we take the pendulum to be a typical representative of deterministic systems, we can say that they are expected to have the following characteristic features:

1. Their dynamic behavior should be *completely predictable* given the equa. tions and a set of initial conditions.
2. Small variations in the initial conditions should have very little effect on the system trajectories.
3. The *attractors* in such systems should be relatively simple geometric forms (equilibria, for example, are points).

It turns out that chaotic systems do not possess *any* of these properties although they are deterministic systems in their own right. Their dynamic behavior is *unpredictable*, they are *hypersensitive* to changes in initial conditions, and their attractors are *geometrically complex* figures. This is completely unexpected, since the equations that describe them are precisely defined and contain no random elements.

![fig2-05](ch02/ch02-fig2-05.png)
#### Fig. 2.5 A system with multiple attractors

To illustrate this point, in __Fig. 2.6__ we show the temporal evolution of one such system, which is used to model the behavior of atmospheric processes. The trajectory depicted in this graph gives no indication whatsoever of any regularity or predictability.

In addition to having random-looking trajectories like the one in __Fig. 2.6__, chaotic systems can also exhibit a property known as *intermittency*, which allows for sudden and completely unexpected aperiodic bursts that interrupt long periods of orderly behavior. In __Fig. 2.7__ we show an example of such a burst, which is associated with the so-called logistic map* (this is a simple equation that has been used for studying a wide range of phenomena, including financial markets, chemical reactions, moth colonies and even human physiology).

![fig2-06](ch02/ch02-fig2-06.png)
#### Fig. 2.6 The trajectory of a chaotic system

Perhaps the most striking aspect of intermittent dynamics is the fact that the aperiodic episodes are essentially unrepeatable, and cannot be predicted from the equations that describe the process. The possibility that a deterministic system could behave in such a way brings into question some widely held assumptions about natural phenomena and the laws that govern them. Indeed, it is conceivable that entire generations of observers could register only the regular dynamic pattern, with no idea that other forms of behavior are even possible. From an empirical standpoint, what we have here are “laws” that can occasionally be “broken”, although the underlying equations are no less precise than those of Newtonian physics.

![fig2-07](ch02/ch02-fig2-07.png)
#### Fig. 2.7 A system with multiple attractors

To complicate matters even further, we should note that chaotic systems are extraordinarily sensitive to changes in external parameter. Meteorologist Edward Lorenz first observed this phenomenon in 1961, while studying a simple model for weather prediction. In repeating one of his computer simulation, he happened to round-off of the initial conditions at the fourth decimal place, fully expecting that this would have no significant effect on the calculations. To his surprise, Lorenz found that the new result was completely different from the old one. He subsequently named this phenomenon the “butterfly effect,” a term that underscores the possibility that something as insignificant as the movement of a butterfly’s wings could ultimately affect global weather patterns.

The extent of the sensitivity exhibit by chaotic systems is illustrated in __Fig. 2.8__, where we compare two trajectories whose initial values differed by one millionth of one percent (for better clarity, the trajectories are represented by lines of different thickness). It is readily observed that the two solutions are identical at first, but bear no resemblance to teach other after a sufficiently long time. This is precisely the kind of dynamic behavior that characterizes atmospheric phenomena, which explains why long term weather forecasts tend to be inaccurate.

![fig2-08](ch02/ch02-fig08.png)
#### Fig. 2.8 Evolution of two initially close solutions.

In the face of such inherent uncertainty, can we say anything concrete about the behavior of chaotic systems? It turns out that we can. While we cannot precisely anticipate what such a system will do, we *can* establish certain limits regarding what is possible. These limits may be difficult to see if we plot the temporal evolution of the variables, but a graph like the one shown in __Fig. 2.4__ reveals that there is some order in chaos. It becomes, clear, for instance, that such systems *do* have attractors, but with geometric properties that are far more complex than the ones we have encountered so far. An example of such a *strange attractor* is shown in __Fig. 2.9__ (this particular attractor corresponds to a nonlinear electric circuit). It is interesting to note that although various trajectories traverse this unusual geometric form in unpredictable ways, the difference between them is necessarily *bounded* (since they are all confined to the attractor). THis places a strict limit on the range of possible responses, although we cannot specify the exact path that the system will follow.

![fig2-09](ch02/ch02-fig09.png)
#### Fig. 2.9 Example of a strange attractor.

The fact that deterministic physical models can sometimes give rise to unpredictable dynamic behavior has important consequences for our understanding of science and its methods of investigation. To begin with, we must allow for the possibility that certain types of complex systems cannot be analyzed using standard experimental techniques. To see why this si so, it suffices to recall that classical physics implicitly assumes that all experiments are *repeatable*. This cannot be guaranteed in the case of chaotic phenomena, where even the smallest variation in external conditions can completely alter the outcome.

THe hypersensitivity associated with chaos points to a second difficulty which is related to the modeling of complex physical processes,. If we acknowledge that there are systems whose sensitivity to external influences is infinite (as chaos theory suggests), then there will be instances where it is virtually impossible to distinguish between important and unimportant parameters in the model. In such cases we would have to take the *entire* environment into account, down to the last atom in the most remote corner of the universe. This is clearly a task that exceeds our computational capabilities (and even our imagination).

If standard techniques such as laboratory experiments and numerical simulations fail to provide adequate information about complex phenomena, what other options do we have for describing them? At present, there is no clear answer to this question. The only thing that we can state with reasonable confidence is that the study of complex systems will probably require the development of new kinds of laws, which may not be as “binding” as the ones we are used to. Needless to day, this possibility has interesting theological implications, which we will explore in Chapter 10.