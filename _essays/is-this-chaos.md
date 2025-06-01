---
layout: post
title:  "Is This Chaos?"
date: 2023-02-10 07:00:00 +0100
published: false
usemathjax: true
---

After our meeting at Leominster on Monday 13th Jan I thought about why I argued a pencil balanced on it's tip is unstable and unpredictable, but not chaotic. I checked online and and found this quotation on wikipedia. <https://en.wikipedia.org/wiki/Chaos_theory#Introduction>. I am finding it difficult to argue Lorenz's case without wandering into realms of pure mathematics.

> ***A Popular but Inaccurate Analogy for Chaos***

> The sensitive dependence on initial conditions (i.e., butterfly effect) has been illustrated using the following folklore:

> *For want of a nail, the shoe was lost.*

> *For want of a shoe, the horse was lost.*

> *For want of a horse, the rider was lost.*

> *For want of a rider, the battle was lost.*

> *For want of a battle, the kingdom was lost.*

> *And all for the want of a horseshoe nail.*

> Based on the above, many people mistakenly believe that the impact of a tiny initial perturbation monotonically increases with time and that any tiny perturbation can eventually produce a large impact on numerical integrations. However, in 2008, Prof. Lorenz stated that he did not feel that this verse described true chaos but that it better illustrated the simpler phenomenon of instability and that the verse implicitly suggests that subsequent small events will not reverse the outcome (Lorenz, 2008 ). Based on the analysis, the verse only indicates divergence, not boundedness. Boundedness is important for the finite size of a butterfly pattern. 

The key phrase here is: "the verse only indicates divergence, not boundedness". "Boundedness is important for the finite size of a butterfly pattern". I believe the boundedness of a chaotic system is a mathematical property of the model, not the system being modelled. It means that there are maximum and minimum values for the possible output of the system. 

A list of chaotic systems may include forced pendulums, resonantly vibrating components of your motor car, the frequency of drips from a faulty tap, the frequency of sunspots, the motion of the jetstream and so on. There is a sense in which they are all bounded; the pendulum on it's string, the chaotic vibration of a part of your car ceases when the part falls off. It cannot move beyond the car. The drips from a faulty tap remain in the basin, Sunspots remain on the the surface of the sun. The jetstream remains in the upper apmosphere.

A list of random events may include the score on a pinball machine, the score of a dice, whether a coin comes up head or tails at the start of football match, or the whereabouts of confetti scattered on a windless day. These outcomes are all bounded in the sense that a dice can only produce the values 1 to 6, the toss of a coin is limited to the values H or T, 

I can find an attractor for models of the first group. For the second group I can find bounds for the list of possible outcomes and the probability of each outcome. I cannot demonstrate that this difference is anything more than a lack of mathematical acumen.

I think I have to wander into realms of mathematics and quote wholesale from 'The Encyclopedia of Mathematics' <https://encyclopediaofmath.org/wiki/Chaos>

> ***deterministic chaos***

>Chaos describes a situation where typical solutions (or orbits) of a differential equation (or typical evolutions of some other model describing deterministic evolution) do not converge to a stationary or periodic function (of time) but continue to exhibit a seemingly unpredictable behaviour. There are different ways to formalize this notion mathematically. Below one such a formalization will be considered, followed by a discussion of some examples.

>The dynamical systems (or models describing deterministic evolution, cf. Dynamical system) considered are differential equations \\( \dot{x} \\)=F(x)
, with x∈X, X a differentiable manifold and F:X→T(X) a vector field on X, and differentiable mappings ϕ:X→X which may or may not be invertible. For a given initial state x0∈X, the corresponding evolution is the solution x(t) of the differential equation with x(0)=x0 or, in the case of a mapping, the function N→X given by n↦ϕn(x0). The last case is the discrete-time situation, the first case that of continuous time. Even if the evolutions can be defined for negative time, only the part with positive time is considered. Also, only bounded evolutions are considered here, i.e. evolutions x(t), xn, with t≥0, respectively n≥0, whose closure, as a subset of X, is compact. It is assumed that there is a metric defined on X

.

One says that such a dynamical system is chaotic if there is a subset X˜⊂X
which has positive measure (for every measure in the Lebesgue measure class) which is invariant in the sense that every evolution starting in X˜ stays in X˜, and such that the evolutions in X˜

have the following properties:

1) no evolution starting in X˜
is periodic or quasi-periodic; an evolution x(t) is quasi-periodic if it can be written as x(t)=F(ω1t…ωmt) with ω1…ωm independent over the rationals and F periodic with period 1 in all its variables, an evolution xn is quasi-periodic if it can be written as xm=F(ω1n…ωmn) with 1,ω1…ωm independent over the rationals and F

periodic with period 1 in all its variables;

2) no evolution in X˜

tends to a periodic or quasi-periodic evolution as time tends to infinity;

3) (sensitive dependence on initial conditions) there is some positive constant A
such that for each x0∈X˜ and each ϵ>0, there is some y0, in an ϵ- neighbourhood of x0, such that for some positive time the evolutions starting in x0 and y0 are more than A

apart.

These conditions are probably not independent: the first two conditions may be a consequence of the third condition, but this has not been proved (1988). The third condition implies some inpredictability. Even if one knows the initial state with arbitrary (but finite) precision, there is some moment in the future at which the state cannot be predicted within a distance A

from the information about the initial state.

General references for this area are [a1] and [a4].

The main examples of chaotic dynamical systems (and dynamical systems which are supposed to be chaotic) are discussed below.

1) The logistic family. This is a one-parameter family of one-dimensional mappings: La(x)=1−ax2
. It has been proved that for a large set (of positive Lebesgue measure) of values of the parameter a

, this mapping defines a chaotic dynamical system. These mappings were introduced to describe population dynamics under certain conditions. A general reference is [a3].

2) The Hénon family [a5]. This is a two-parameter family of two-dimensional invertible mappings Ha,b(x,y)=(1−ax2+y,bx)
, b≠0. In this example there is only numerical evidence that Ha,b defines, for many parameter values a and b

, a chaotic dynamical system. The mathematical analysis of this example is still in progress (1988).

3) The Lorenz family [a6]. This is a three-parameter family of differential equations in R3

:

x˙= σ(y−x),

y˙=rx−y−xz,

z˙=xy−bz.

There is a well-developed theory concerning this system. Still, there is no complete proof that for any of the parameter values this system is chaotic. This chaoticity is strongly suggested by numerical results combined with geometric arguments: what is lacking is a tedious numerical verification. This equation was proposed in connection with convection problems.

4) General (non-trivial) Axiom A

attractors. This is a class of abstract dynamical systems which are chaotic. Among the chaotic dynamical systems they are the most "regular" and also they are the ones which are mathematically well understood, see [a2].

Finally, in a number of physical and chemical experiments, in particular related with weak turbulence and open chemical reactions far from equilibrium, the experimental data indicate that one should explain these experiments in terms of chaotic dynamical systems, see [a1].

The literature has not yet standardized with respect to the definition of chaotic mappings. Thus, in [a7] the discrete-time system on V
given by f:V→V is said to be chaotic if (i) f has sensitive dependence on initial conditions; (ii) f is topologically transitive, i.e. for every open U1,U2⊂V there is an n>0 such that fn(U1)∩U2≠∅; and (iii) the periodic points are dense in V. 

