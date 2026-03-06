---
publish: true
created: 2026-03-05T17:29:11.211-05:00
modified: 2026-03-05T21:24:24.490-05:00
tags:
  - lecture
  - S2
  - me274
cssclasses: ""
---

# Linear Impulse-Momentum Equation for a Single Particle
$$m\vec{v}_{2}=m\vec{v}_{1}+\int  _{1}^2 \vec{R}~ d{t}$$
where $m\vec{v}$ is the *linear momentum* of the particle and $\int _1^2\vec{R}~ d{t}$ is the *impulse* of the net force acting on the particle
1. The above is the impulse-momentum equation for a particle since the equation relates the change in laer momentum to the impulse acting on the particle
2. Note that this equation relates the change in velocity of the particle to a change in time (from $t=t_{1}$ to $t=t_{2}$)
3. In contrast with the work-energy equation, the impulse-momentum is a vector equation, that is, the equation can be resolved into components. For example, if the forces acting on the particle are resolved into a set of $x-y$ Cartesian components, then the above vector equation represents the following two sets of scalar equations:
$$mv_{x2}=mv_{x1}+\int  _{1}^2 R_{x}~ d{t}$$
$$mv_{y2}=mv_{y1}+\int  _{1}^2 R_{y}~ d{t}$$
4. If the resultant force in a given diretion is zero, then linaer momentum is *conserved* in that direction. For example, suppose that $R_{x}=0;$ then from above we see that:
$$mv_{x2}=mv_{x2}\implies v_{x2}=v_{x1}$$
Conservation of momentum in one direction does not imply conservation in any other directions
5. *Conservation of momentum does not imply or result from conservation of energy.* Momentum and energy are two independent quantities
# Impulse-Momentum Equation for a System of Particles
$$\sum m_{j}\vec{v}_{j2}=\sum m_{j}\vec{v}_{j1}+\int  _{1} ^2 \left[ \sum \vec{F}_{j}^{ext} \right]~ d{t}$$
where $\sum m_{j}\vec{v}_{j}$ is the total linear momentum of the system and $\sum \vec{F}_{j}^{ext}$ is the resultant external force acting on the $j$th particle
1. Recall that the above equation results from the summation of impulse-momentum equation for each particle in the system. An important result of this is that *internal* forces cancel, and the impulse due to only the *external* forces contributes to the change of the total linear momentum of the system
2. It is advisable to make your choice of the system to be as large as possibly to make as many forces *internal* to the system as possible. However, remember than any force that is internal to the system cannot be determined from this equation
3. As before, note that the linear impulse-momentum equation is a vector equation
4. Linear momentum for a system, in a given direction, is conserved when the net external forces in that direction is zero. When working problems with the impulse-momentum equations, draw the FBD of your system: look for directions in which there are no net forces. In these directions, you can use conservation of linear momentum

>[!example] A tug having a mass of $m$ is towing a coal barge (mass $M$) with a speed of $v_{A1}$. During a short period of time $\Delta t$ whne the engines of the tug are turned off, the stern wenchtakes in the towing cable at a rate of $v_{B/A}$. Determine (a) the speed of the tug during this time; (b) the average value of the tension in the towing cable during this time. Ignore water resistance on the tug and barge, also assume that the towing cable remains taut at all times. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=240|figure]]
>*[[Pasted image 20260305184829.png|FBD (a)]], [[Pasted image 20260305190103.png|FBD (b)]]*
>**Kinetics:**
> $$\text{Since }\sum F_{x}=0,\text{ linear momentum is conserved in }x\text{-direction}$$
> $$mv_{A1}+mv_{B1}+\int  _{1}^2 \cancel{ F_{x} } d{t}=mv_{A2}+mv_{B2}$$
> $$v_{A1}=v_{B1}\text{ so }(m+M)v_{A1}=mv_{A2}+mv_{B2}$$
> $$v_{B2}=v_{A2}+v_{B/A}\to (m+M)v_{A1}=(m+M)v_{A2}+mv_{B/A}$$
> $$\text{(a) }\textcolor{green}{v_{A2}=v_{A1}-\frac{m}{M+m}v_{B/A}}$$
> $$\text{In x-direction: }mv_{A1}+\int  _{1}^2 T~ d{t}=mv_{A2}\to mv_{A1}+T\Delta t=mv_{A2}$$
> $$\text{(b) } \textcolor{green}{T=\frac{m(v_{A2}-v_{A1})}{\Delta t}}$$

>[!example] Block $P$, weighing 100lb, is initially stationary when a force $F(t)$ begins acting on it, with $F(t)$ given in the graph shown. The coefficients of static and kinetic friction between the block and horizontal surface on which it moves are known to be $\mu_{s}=0.5,\mu_{k}=0.2$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=239|figures]]
>*[[Pasted image 20260305190612.png|FBD]]*
>**Kinetics:**
>$$F_{s,max}=\mu_{s}N=\mu_{s}W=50\text{lb},\text{ since }F(t)=20t,f_{s}\text{ is maximized at }t=2.5\text{s}$$
> $$\text{in }x\text{-direction: }mv_{1}+\int  _{1}^2 (F-f)~ d{t}=mv_{2}$$
> $$\text{When does the block begin to move? }F_{s,max}=\mu_{s}N;\sum F_{y}=N-W=0\text{ so }F_{s,max}=\mu_{s}W=50\text{lb}$$
> $$\cancel{ mv_{1} }+\int  _{2.5\text{s}} ^{10\text{s}} \left( 20\frac{\text{lb}}{\text{s}} -\mu_{k}W\right)~ d{t}=mv_{2}$$
> $$\left. 10 \frac{\text{lb}}{\text{s}}\cdot t^2-20\text{lb}\cdot t~ \right|^{10\text{s}} _{2.5\text{s}}=787.5\text{lb}\cdot\text{s}$$
> $$m=\frac{W}{g},m=3.11 \frac{\text{lb}\cdot s^2}{\text{ft}}\to \textcolor{green}{v_{2}=253.4\text{ft/s}}$$

