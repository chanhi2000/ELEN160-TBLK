## 2.3 Complexity and Self-Organization

The phenomenon of chaos is intimately related to the notion of *complexity* and *self-organization*, and this collection is worth examining in some detail. Given that complexity is a notoriously ambiguous word, it makes sense to begin our discussion with an appropriate definition. This is by no means easy, Since there are a number of competing interpretations in current use. In computer science, for example, the term “complexity” is usually associated with the length of the shortest program that can produce a particular data set. If we adopt that definition, a number such as $$\pi$$ could be viewed as relatively “simple,” since there are explicit formulas that allow us to compute its decimal digits. Because such formulas exist, the same short program could be used to produce the first $$5$$ or the first $$100,000$$ decimal of this number.

In contrast to $$\pi$$, there is an abundance of real numbers whose decimal digits exhibit *no* pattern whatsoever. Such numbers are said to have high *algorithmic information complexity*, since each decimal digit needs to be described *separately*. This means (among other things) that the program needed to produce the first $$5$$ decimal digits would be fairly short, but the one needed for the first $$100,000$$ decimals would be extremely long. The program length would obviously continue to grow if we were to increase the desired number of decimals, with no upper limit in sight.

While the above definition appears to be perfectly acceptable in information theory, it clearly deviates from what we normally mean when we use the attribute “complex.”

> “Compare a play by Shakespeare with the typical product, of equal length, of the proverbial ape at the typewriter, who types every letter with equal probability. The algorithmic information complexity, or algorithmic randomness, of the latter is overwhelmingly likely to be greater than that of the former. But it is absurd to say that the ape has produced something more complex than the work of Shakespeare.” *Murray Gell-Mann*[^3]

To this we might add the observation that random data can often be represented in compact form, despite the fact that it cannot be reproduced by a simple program. A typical example of this sort is so-called “white noise,” which is completely random but can nevertheless be described in terms of only two pieces of information—the mean and the standard deviation, with that in mind, it seems reasonable to treat *both* strictly regular *and* strictly irregular data as essentially “simple”, while viewing data that lies somewhere in between as “complex”. Complexity understood in this way can be directly associated with phenomena such as chaos, which have both orderly and unpredictable features.

The same combination of order and disorder that characterizes chaotic behavior also plays a crucial role in the process of *self-organization*. Recent research suggests that complex systems (both of the animate and inanimate variety) seem to "prefer operating at the edge of chaos, where the range of possible configurations is virtually unlimited. Such “openness” to change, combined with an extraordinary sensitivity to external stimuli, is an essential prerequisite for the emergence of novelty in nature.

It goes without saying, of course, that novelty alone doesn’t automatically imply an increase in complexity (or even functionality, for that matter). Evolutionary biology makes this point in no uncertain terms. Nevertheless, the sheer number of possible outcomes that exist at the "edge of chaos” makes it very likely that some of them will ultimately lead to higher forms of organization. More often than not, such “advanced” forms arise spontaneously, as a result of simple local interactions between autonomous agents. These interactions tend to occur without any form of global coordination, which is why they are commonly associated with the process of self-organization.

Phenomena of this sort are usually characterized by one or more threshold values, which separate the domains of “ordinary” and “critical” behavior. The term “critical implies (among other things) that small disturbances in the system can have unpredictable consequences. As an illustration of this property. imagine a large object that is being pushed across a smooth surface (such as ice, for example). In that case, energy will be dissipated at the same rate at which it is added to the system, and the motion of the object will be *continuous*. If, on the other hand, the surface happens to be rough, energy could be added to the system for quite a while without causing any motion at all. However, When a threshold value is reached, the accumulated energy dissipates through an abrupt, *discontinuous* movement. States in which a force is ied but the object remains motionless are external disturbances When the system is in such a state (which corresponds to the “edge of chaos”), a small increase in the applied force can bring about almost kind of response — a small movement, a large one, or even no movement at all. It is this combination of unpredictability and hypersensitivity that creates the necessary conditions for novelty and increased complexity.

Among the many instances of spontaneous self-organization in nature, the ones that arise in biology are perhaps the most king. We do not have to look too far up the evolutionary chain to find evidence of such processes. Certain types of molds, for example, produce amoeba-like cells that tend to “cluster together” when the food supply become in the concentration of a chemical substance known as ascrasin, which is secreted by the cells when there is a shortage of food. Interestingly each cell that encounters such a marker begins to produce its own “acrasin trail,” thus amplifying the local chemical signal. The end result of this process is an aggregation of cells that resembles a rather large slug-like creature, which is a more complex and qualitatively different organizational form.

An important aspect of this example is the complete absence of any global coordination among the cells. The secretion and detection of chemical signals are essentially forms of *local* interaction, which ultimately give rises to a higher-level structure. Something similar happens when termites construct their mounds, or when ants create swarms (whose length can be up to several hundred meters). In both cases, the individual ants have no way of knowing that they are part of *a larger unit*—they simply follow a chemical trail left immediate vicinity.

> “There is no one ant that is calling the shots, picking from among all the other ants which one is going to get to do its thing. Rather. each ant has a very rest i set of behaviors. ... When one takes these behaviors on aggregate, the whole collection of ants exhibits a behavior, at the level of the colony itself, which is close to being intelligent. ... A collective pattern takes over the population, endowing the whole with models of behavior far beyond the simple sum of the behaviors of its constituent individuals.” *Christopher Langton*[^4]

It is interesting to note that the organizational patterns exhibited by both the molds and the ants have been successfully reproduced by computer-aided simulation.[^5]  In all cases, the programs were based on very simple forms of local on individual agents, but the overall system exhibited complex dynamic behavior. Computer models based on simple local rules were also found to be effective in the study of gene regulation. Pioneering work in this field. was performed by biologist Stuart Kauffman, who introduced *random Boolean networks* as a theoretical tool for modeling this process.[^6] A Boolean network can be viewed as a collection of N interconnected modes (interpreted in this case as genes), which are capable of activating and deactivating each other according to a set of preassigned rules. Despite its apparent simplicity, this mathematical framework proved to be very useful in describing biological systems, and has produced predictions that are remarkably consistent with observed patterns of cell differentiation in living organisms.

To get a better sense for how Boolean networks operate, in __Fig. 2.12__, we provide a simple schematic illustration of such a system. Note that each node in __Fig. 2.12__ has both *incoming* and *outgoing* edges, whose directions  reflect the flow of information in the network. The information exchange between the nodes is strictly local, and there is no global coordination (which is typical for systems that are capable of self-organization)

![fig2-12](ch02/ch02-fig12.png)
#### Fig. 2.12. Example of a Boolean network.

The modes in a Boolean network can be viewed as *autonomous agents*, which act independently in response to external stimuli. It is usually assumed that the state of each node evolves discretely over a series of time steps. In mathematical terms, this means that the next action of node $$i$$ can be described as
$$
x_i(k+1)=F_i(x(k))\tag{2.6}
$$

where vector $$x(k)=\left[x_1(k),\cdots{x}_N(k)\right]$$ represents the current states of all neighboring modes that affect it. It is important to recognize in this context that functions $$F_i\:(i=1,\:2,\:\cdots,\:N)$$ are Boolean, which means that the only values they can produce are $$0$$ or $$1$$. It is easily verified that any such function can be defined in the form of a look-up table, which is convenient from the standpoint of computer-aided simulation.

Assuming that each of the $$N$$ nodes has exactly $$K$$ incoming edges, there are many possible ways for assembling a Boolean network (each such configuration represents a “realization” of the $$N\:K$$ network). In addition to selecting an interconnection pattern, one can also assign a different function $$F_i$$, to each mode and choose a set of initial conditions. When all these options are taken into unt, the number of possibilities can reach staggering proportions. For that reason, the study of Boolean networks normally involves a *random* sampling of different configurations (hence the name “random Boolean networks”).

In order to see how connectivity affects the process of gene regulation, Kauffman studied the average number and length of independent periodic patterns (so-called *limit cycles*) that arise in an ensemble of randomly chosen $$N\:K$$ networks. His experiments showed that when each gene interacts with only *one* neighbor (*i.e.* when $$K=1$$), the system dynamics become rather uninteresting with a tendency of converging to a fixed set. On the other hand, if genes were allowed to exchange information with all other genes (*i.e.* when $$K=N$$). the patterns were found to be extraordinarily complicated and hypersensitive to perturbations. In most such cases, the overall system behav SOWed Tlso signs of regularity. At the transition between these two rather extreme regimes, Kauffman identified a region of “critical” behavior, which is characterized by a mixture of order and disorder. He referred to this region as the “edge of chaos,” and suggested that such complex dynamics proνίde a natural mechanism for the process of self-organization in biological systems.[^7]

The patterns associated with Boolean networks that operate at the "edge of chaos" highlight the importance of local interactions, and point to *complexity* as a necessary condition for information processing on the cellular level. Indeed, when the system is “static” (as in the case of $$K=1$$), information can be stored but cannot be manipulated in any meaningful way. On the other hand, systems that change very easily (such as those with $$K=N$$) are capable of processing information, but are too dynamically active to allow for any kind of memory. The complex behavior that occurs for the critical value $$K=2$$ seems to provide just the right balance of order and uncertainty that enables the nodes to transmit, modify and retain information (which is what genes are presumably supposed to do).[^8]

What can we conclude from this discussion? Based on the examples considered above, it would appear that new and increasingly complex structures can arise spontaneously in nature, simply as a result of local interactions between autonomous agents. This type of self-organization does not require a “masterplan,” or any other form of global control.

The fact that such processes are closely associated with chaos further indicates that a mixture of order and uncertainty is essential for the emergence of novelty in mature. Indeed, if all physical processes were as orderly and predictable as the movement of a pendulum, it is highly unlikely that life as we know it would ever have developed. Fortunately for us, the universe seems to be a far more interesting place than physicists of the 18th and 19th centuries had anticipated. What we have learned about chaos and complexity in recent years suggests that mature is still a “work in progress”, whose future states are by no means predetermined. From that perspective, it is perhaps best to view physical environment as a vast array of possibilities, not all of which will be realized. We will see in Chapter 10 that such a view has important consequences for the theological understanding of evolution and the origins of the universe.

[^3]: Murray Gell-Mann, “Regularities and Randomness: Evolving Schemata in Science and in the Arts,” in Casti and Karlovist (Eds.), *Art and Complexity*.
[^4]: Quoted in: Charles Birch, “Neo-Darwinism, Self-Organization and Divine Action in Evolution,” in *Evolutionary and Molecular Biology*, R. J. Russell, W. R. Stoeger and F. J. Ayala (Eds.), Vatican Observatory Publications, 1998.
[^5]: See *e.g.* Mitchell Resnick, “Learning About Life,” in *Artificial Life: An Overview*, Christopher Langton (Ed.), MIT Press, 1995. Another interesting article on this subject is: Nigel Franks, “Army Ants: A Collective Intelligence,” *Scientific American*, 77, pp. 139-145.
[^6]: Stuart Kauffman, *Origins of Order: Self Organization and Selection in Evolution*, Oxford University Press, 1993.
[^7]: Ibid.
[^8]: An interpretation of Boolean networks which links complexity and information processing can be found in: Gary Flake, *The Computational Beauty of Nature*, MT Press, 2000