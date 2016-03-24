# Faith, Reason and Analogical Thinking

## Analogies, Probability and Plausibility
In thinking about what constitutes a “rational" belief system, it is useful to recognize that our actions and opinions are guided by what physicist (and historian of science) Gerald Holton describes as a “robust, map-like constellation of .., beliefs about how the world as a whole operates.” He refers to this overall outlook that shapes our attitudes as our Weltbild (which is a somewhat broader German term for “world view")[^9]. Although the Weltbild of any given individual depends to a large extent on his social, ethnic and educational background al fair to say that it always contains a subset of beliefs that pertain to the natural world. It is perhaps here that we might locate an appropriate meaning for the attribute “rational,” at least when it comes to scientifically minded individuals I would suggest that for such a person, a coherent world view would be one satisfies the following two conditions:
1. The set of “core” beliefs about the natural world must to be Compatible with existing scientific knowledge.
2. The “non-scientific” core beliefs should be consistent (at least in some measure) with the scientific ones.

In applying these criteria, it is important to keep in mind that the term “consistent” must be used somewhat loosely. Indeed, I seriously doubt that the entire mindset of any individual could pass a strict test of logical soundness (which is perhaps what makes us human in the first place). With that in mind, I would argue that the rationality of our Weltbild can be justified by establishing appropriate “logical bridges” between the disparate clusters of views that constitute it. Formal proofs are of little use in this enterprise, and should ultimately give way to analogies and metaphors.

What is it about analogies and metaphors that makes them so suitable for this purpose? Our primary motive for focusing on these two modes of description stems from the fact that they have always been a natural tool for explaining difficult concepts, both in science and in theology. If these two disciplines are seen as manifestations of the same overarching reality (as Christian theology suggests), then it is perfectly reasonable to assume that analogies can also help bridge the apparent gap that separates them. From a theological perspective, what we are really proposing here amounts to adding a certain number of “scientific" metaphors to the already existing traditional ones. The potential value of such metaphors has been recognized by several contemporary thinkers:

> "Metaphors fund theology, providing the language and images out of which theological concepts grow; they describe the unknown in terms of the known. ... When metaphors lose their original meaning and fruitfulness, the theology built upon them must be reconstructed, drawing upon new metaphors appropriate for a new age... It seems reasonable that physics, as well as biology and the other sciences which infuse our culture, can be a source of religious metaphors.” Robert J. Russell [^10]

> “For religion to be able to meet the needs of its day (to answer the question of meaning) it must be in accord with, and understandable in the language of the scientific knowledge of the time.” Wallace Clift [^11]

Before proceeding down this path, it is worth considering whether analogical interpretations carry any weight in the domains of science and mathematics (beyond the indisputable educational value that they posses). It turns out that they do. An obvious example of this kind arises in the context of formal logic, where “interpretations” allow us to establish the consistency of abstract systems, and determine the truth (or falsity) of purely symbolic statements. To get a sense for how this works, consider the apparently random string of characters $$\text{NNNPNQNN}$$ and ask yourself whether this can be a “true” statement in some formal system. There is obviously no way to tell, unless we attach some to these symbols. The interpretation provided in Table 1.1 suggests one possibility, which allows us to “translate” our string into a true statement about integers (i.e. $$3+1>2$$). Based on this analogy between the symbols N, P and Q and the elements of number theory, we can conclude that $$\text{NNNPNQNN}$$ can indeed be a “theorem” (the formal basis for this claim is provided in Chapter 3).

| symbol | interpretation |
| :----: | :------------: |
| $$\text{P}$$ | $$+$$ |
| $$\text{Q}$$ | $$>$$ |
| $$\text{N}$$ | $$1$$ |
| $$\text{NN}$$ | $$2$$ |
| $$\text{NNN}$$ | $$3$$ |
###### Table 1.1 A possible interpretation of the symbols

Although such a precise procedure is clearly impossible to reproduce in the case of theology, one could nevertheless argue that analogies perform a similar function. Indeed, their primary purpose is (and always has been) the “translation” of complex and counterintuitive theological claims into a more manageable framework. If this framework happens to be math or science, a careful choice of analogies could provide some new (and possibly unexpected) insight about certain religious beliefs, and could perhaps help us reconcile them with the scientific elements of our *Weltbild*.

Analogies between scientific and theological concepts can also be to establish the plausibility of certain contentious religious propositions, which is a necessary step in justifying their rationality. To see why “more plausibility” " is sufficient for this purpose, we must make a brief excursion into probability theory, and examine how cumulative evidence can affect our evaluation of competing hypotheses. We begin with the observation that the notion of probability is often related to the relative frequency with which certain outcomes occur. When we say, for example, that the probability of drawing a particular card from a standard deck is $$P=\tfrac{1}{52}=0.019$$, it is implicitly assumed that the experiment will be repeated many times (which is typically the case in science). Thus, if we were to attempt 1,000 independent draws, the probability calculated above suggests that we should expect 19 of them to produce, say, the ace of spades.

It is obvious, however, that this interpretation doesn't work particularly well in the domain of religion, where non-repeatable situations are a common occurrence. In order to extend the notion of probability to phenomena that do lend themselves to repeated experimentation, we need to think of it as a of how strongly we believe in a proposition (or a hypothesis). Any such situation must necessarily take into account available evidence, and the fact that probabilities are different before and after an event occurs. These probabilities are related by Bayes’ theorem, which states that
$$
P(HE)=P(E|H)P(H)
$$
where
1. $$P(H)$$ is the probability that hypothesis $$H$$ is true before event $$E$$ Occurred (the so-called prior probability).
2. $$P(H|E)$$ is the probability that $$H$$ is true after event $$E$$ occurred (also known as the posterior probability).
3. $$P(E|H)$$ is the probability that event $$E$$ will take place if $$H$$ is true.

To gain a better understanding of what this theorem really means, let us consider a simple example which examines whether it is ‘reasonable to believe in the existence of the Loch Ness monster.[^12]

#### Example 1.1.
In the case of the Loch Ness monster, there appear to be only two possible hypotheses:
- $$H_1$$ : The monster exists.
- $$H_2$$ : The monster does not exist.

If we are inclined to believe (as many are) that the monster story is no more than a myth, we will assign a small probability to hypothesis Hı. For illustrative purposes, suppose we have decided that $$P(H_1)=0.01$$ and $$P(H_2)=0.9$$ which is equivalent to assuming that the odds are initially $$99:1$$ in favor of hypothesis $$H_2$$. What kind of evidence would be needed to substantially change these odds? To see that, let us assume that a moving Serpent-like shape was observed (and photographed) in the lake by a team of scientists who happened to be flying over. in a helicopter. In the following, we will refer to this sighting as event $$E_1$$.

In order to apply Bayes' rule, we must first determine probabilities $$P(E_1|H_1)$$ and $$P(E_1|H_2)$$ (i.e. the probabilities that event $$E_1$$ would take place given each of the two hypotheses). If we assume that the monster exists, it is by no means surprising that event $$E_1$$ should occur, which means that we can assign a rather large value to probability $$P(E_1|H_1)$$. If, on the other hand, we assume that there is no monster, the sighting would be quite surprising, and we could associate a fairly low value with $$P(E_1|H_2)$$ (not too low, however, since we must allow for optical illusions, faulty equipment, etc.).

For the sake of argument, let us suppose that $$P(E_1|H_1)=0.9$$ and $$P(E_1|H_2)=0.1$$. According to Bayes’ theorem, the probabilities of the two hypotheses after event $$E_1$$ took place will change to $$P(H_1|E_1)=0.009$$ and $$P(H_2|E_1)=0.099$$, respectively, and the odds become $$11:1$$ in favor of $$H_2$$. Based on these odds, it is still much more likely that the monster is a mythical creature, but the discrepancy between the two hypotheses is dramatically lower than it initially was.

Let us now consider a scenario where not one, but rather two independent events occur: $$E_1$$ (the same event that was described above) and $$E_2$$ (a large moving object has been detected at the bottom of the lake using a sonar). Since there is no correlation between the two events, it can be shown that the odds are now reduced to only $$1.2:1$$ in favor of $$H_2$$. In other words, after these two observations (each of them inconclusive), the two hypotheses have become almost equally likely, despite the very large initial difference.

What can we conclude from this example? The “moral” of the story is that cumulative evidence can dramatically alter the odds in favor of some hypothesis, no matter how unlikely it may have seemed at the outset. The only scenario where this conclusion fails to apply is when $$P(H)=0$$. This would be the case, for example, if the hypothesis is self-contradicting, or is in direct conflict with established scientific facts. Under such circumstances, all evidence becomes irrelevant and can be dismissed a priori.

Arguments based on the fact that $$P(H)$$ can be zero have been quite popular among secular thinkers, who maintain that some religious claims are simply too outrageous, and cannot be reconciled with established scientific knowledge. It is largely for this reason that it is fundamentally important to show that certain counterintuitive theological teachings could *conceivably be true*. This is where analogies with science can be particularly useful - they can help establish the plausibility of such propositions, thereby ensuring that we can assign a non-zero prior probability to them. Then (and only then) can we include evidence such as historical testimonials and accounts of mystical experiences, and use it to justify the rationality of religious beliefs.

[^9]: Gerald Holton, Science and Anti-Science, Harvard University Press, 1997.
[^10]: Quoted in: Russell et. al. (Eds.), Physics, Philosophy and Theology
[^11]: Wallace Clift, Jung and Christianity, Crossroads, 1986.
[^12]: This example represents a variant of the one described in David Bartholomew, Uncertain Belief, Oxford University Press 2000.
