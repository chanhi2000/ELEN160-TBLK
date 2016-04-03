## 3.1 What Is a Formal System?

The ‘axiomatic’ approach to mathematics dates back to ancient Greece and the development of geometry. The starting point of the Greeks was quite simple — they argued that geometry can be based on a number of self-evident propositions that are accepted *without proof*. These propositions are known as *axiom*, and can subsequently be used to derive all other propositions as *theorems*, according to some preset rules.

Around 300 B.C., Euclid set out to systematize all existing knowledge about geometry in a seminal book entitled *The Elements*. He began by formulating the following four ax our everyday experience. 

__AXIOM 1.__ A straight line segment can be drawn joining any two points.

__AXIOM 2.__ Amy straight line segment can be extended indefinitely in a straight line.

__AXIOM 3.__ Given any straight line segment, a cil the segment as radius and one end point as center.

__AXIOM 4.__ A. All right angles are congruent.

From these axioms, the first theorems of geometry were derived directly (they constitute what is known as *absolute geometry*). But there was a catch ... Despite all his efforts, Euclid was unable to prove a proposition that can paraphrased as follows:

__PROPOSITION 5.__ Consider a line $$l$$ and a point $$a$$ that does not belong to it. Then, there is one and only one line that passes through a and does not intersect $$l$$.

Since this statement appeared to be intuitively true, Euclid decided to adopt it as the fifth axiom in his system. All subsequent theorems that followed from this assumption constitute what we now refer to as Euclidean  geometry.

There is no doubt that Euclidean geometry developed into a logically sound system. Since its axioms reflected obvious truths, there was no danger that two theorems would ever contradict each other (a property known as *internal consistency*). Over the years, the practical applicability of Euclidean geometry added to its appeal, and solidified its status as a cornerstone of mathematicians remained troubled by the fifth axiom. Part of the problem stemmed from the belief that human intuition is limited to *finite* objects, and cannot be used to anticipate what may happen at infinity (which is precisely what __Proposition 5__ required). As a result, the two millennia that followed Euclid's death witnessed countless attempts to close the loophole, and derive __Proposition 5__ from the original four axioms. These efforts proved to be unsuccessful, and by the end of the 19th century it was finally established that such a derivation is impossible.

The ‘undecidability’ of __Proposition 5__ turned out to be an enormously important result. Among other things, it was now possible to argue (with full logical justification) that a statement such as the following one can be used as an alternative to __Proposition 5__:

__PROPOSITION 5A.__ Consider a line $$l$$ and a point $$a$$ that does not belong to it. Then, there is *no line* that passes through $$a$$ and does not intersect $$l$$.

The introduction of __Proposition 5A__ as an axiom seems rather bizarre and thoroughly counterintuitive. How can geometry possibly be based on a statement that clearly contradicts our everyday experience? Wouldn’t this be comparable to denying gravity or the rotation of the earth? It certainly would, if we were to adhere to our intuitive notions of a point, line and other basic geometric forms. But what if we were to define a ‘point’ as a *pair* $$(a,\:a_1)$$ of diametrically opposite points on a sphere, and a ‘line $$l$$’ as a *great circle*? In that case, __Proposition 5A__ becomes perfectly reasonable. To see why this is so, consider a line $$l$$ and a point $$(a,\:a_1)$$ that does not belong to it (as shown in __Fig. 3.1__). It is easily verified that any line $$l_1$$ passing through $$(a,\:a_1)$$ must intersect line $$l$$.

#### Fig. 3.1. Generalized motions of a point and line.
![fig3-01](ch03/ch03-fig01.png)

One could argue at this point that axioms such as __Proposition 5A__ may be technically acceptable, but are so abstract that the resulting systems would be completely detached from reality. It turns out, however, that this is not the case. Non-Euclidean geometries have actually found numerous applications, which range from economics to Einstein's theory of general relativity (see Chapter 5 for more details). Developments such as these have lead mathematicians to conclude that axioms needn’t be self-evident truths, or even facts that correspond to our experience. Axioms can actually be pretty much anything, provided that the ensuing theorems do not result in a contradiction.

The recognition that axioms can be chosen in a flexible manner opened the door to the formalization of mathematics. Almost without exception, theoreticians came to believe that all matheematical reasoning could be ultimately represented as a *formal system*, inwhich the axioms and theorems are strings of completely meaningless symbols. Thinking along these lines, the famous philosopher and logician Bertrand Russel came to the conclusion that:

> "Mathematics may be defined as the subject in which we never know what we are talking about, nor whether what we are saying is true." *Bertrand Russel*[^2]

If we agree with Russell that mathematical concepts needn't have any meaning, then the only things that matter are the choice of symbols and the rules by which we manipulate them. Specifying these rules is usually a fairly easy thing to do. It turns out, for example, that describing  a formal system requires only three pieces of information:
__THE RULES OF FORMATION__, which determine wheter or not a string of symbols is a legitimate member of the system.

__THE AXIOMS__, which are "truths" that are accepted without proof.

__THE RULES OF INFERENCE__, which provide the basis for generating new theorems from axioms and already existing theorems.

The following example shows what a simple formal system might look like.[^3]

### Example 3.1. 
(The $$\text{PQ}$$ system). Consider a formal system in which there are only three types of symbols: letters $$P$$, $$Q$$, and strings of hyphens. The system is defined by the rules and axioms described below.

*Rule of Formation*. Any string of the type
$$
x\:P\:y\:Q\:z\tag{3.1}
$$

where $$x$$, $$y$$, and $$z$$ represent sequences of one or more hyphens is a member of this system (we will refer to it as a *well-formed string*).

*Axioms*. Every string of the type
$$
x\:P-Q\:x-\tag{3.2}
$$

where $$x$$ is a sequence of hyphens is an axiom.

*Rule of Inference*. If
$$
x\:P\:y\:Q\:z\tag{3.3}
$$

is a theorem, then
$$
x\:P\:y-Q\:z-\tag{3.4}
$$

is also a theorem

In analyzing the properties of this system, we should first recognize that certain combinations of $$P$$, $$Q$$ and hyphens are *not* allowed in this system. For example,
$$
---P--Q---\tag{3.5}
$$

is a well-formed string, but
$$
---P\:Q---\tag{3.6}
$$

or
$$
-P-Q-P\tag{3.7}
$$

are *not*, since they violate the rule of formation. We should also point out the theorems of the $$\text{PQ}$$ system can be automatically generated from the axioms by applying the rule of inference. Indeed, if we were to start with axiom
$$
--P-Q---\tag{3.8}
$$

the theorem
$$
--P--Q----\tag{3.9}
$$

would follow directly. Applying the rule of inference again, we would get
$$
--P---Q-----\tag{3.10}
$$

and so on. It would actually be quite straightforward to program a computer to generate theorems in this manner. Note, however, that in this c such a program would never terminate, since there are infinitely many axioms and boundless possibilities to produce theorems from them.

The two most important questions that we can ask about any formal system are whether it is *internally consistent*, and whether it is *complete*. What exactly does that mean? For our present purposes, it will suffice to simply describe these concepts, without resorting to precise definitions. We will say that a formal system is internally consistent if its rules of inference ensure that no statement can be *both* true *and* false at the same time. Completeness, on the other hand, will be understood as a property which ensures that every statement in the system can be classified as *either* true *or* false. Note that according to this interpretation, a formal system would be *incomplete* if it contained at least One *undecidable proposition* (*i.e.* a proposition whose “truth status” cannot be established).

Showing that a system is consistent and/or complete can be a formidable task, even in simple cases. If, for example, we were to attempt a proof of Consistency based on the rules of inference alone, our only option would be to generate theorems one by one until we find two that stand in logical opposition. In this way, we might be able to establish *inconsistency* in a finite number of steps (if we are very, very fortunate). Consistency, however, can never be verified in this manner, since infinitely many theorems would need to be examined. It follows, therefore, that such a proof requires some form of reasoning that *transcends* the formal system itself.

A possible way to resolve this problem would be to introduce an *interpretation*, which would allow us to “translate” all the statements of the original formal system into statements about some other (preferably more manageable) system. We already saw how something like this might be done in simple cases (see, for example, __Table 1.1__ in Chapter 1). A somewhat more sophisticated illustration of this process arises in the context of geometry. For centuries it vas assumed that the Euclidean axiomatic si the intuitive nature of its principal propositions. No formal validation of this claim was attempted until the late 1800s, when mathematician David Hilbert proposed a rigorous consis proof. His idea was remarkably simple, and amounted to associating a pair of $$(x,\:y)$$ coordinates with every point in a plane. Such a model allowed him to “translate” every statement of Euclidean geometry into a corresponding algebraic statement, and interpret it accordingly.

The notion of an “interpretation” can be extended well beyond the simple example considered above. A systematic way to do that would be to construct a mapping that assigns a unique integer to each symbol, string and proof of any given formal system. Such an approach seems very promising, since it allows us to “translate” every statement of this system into a corresponding statement about integers, and use the framework of number theory to establish and completeness. It turns out, however, that this path is a erous one. As we shall see, it led to some very surprising result, which ultimately brought into question the very foundations of mathematics.

[^2]: 
[^3]: 
