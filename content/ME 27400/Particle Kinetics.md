---
publish: true
created: 2026-03-03T20:33:39.266-05:00
modified: 2026-03-05T20:02:22.697-05:00
tags:
  - S2
  - lecture
  - me274
  - index
cssclasses: ""
---

# Kinetics: Problem Solving Method
1. **Free body diagrams.** Draw the appropriate free body diagrams for the problem, your choice of which is problem dependent. For some problems, you'll draw an FBD for each body; for others, an FBD for the entire system. Integral part of FBDs is choice of coordinate system. For each FBD, draw unit vectors corresponding to your coordinate choice
2. **Kinetics equations.** Choose what solution method(s) you'll need to use for the particular problem. We'll study Newton/Euler, work/energy, linear impulse/momentum, and angular impulse/momentum
3. **Kinematics.** Perform the needed kinematic analysis. A study of equations in step 2 will guide you in deciding which kinematics are needed for a solution of the problem
4. **Solve.** Count the number of unknowns and number of equations from above. If you don't have enough equations to solve for the unknowns, you either *(i)* need to draw more FBDs, or *(ii)* need to do more kinematic analysis. When you have sufficient equations for the number of unknowns, solve for the desired unknowns from the above equations


**N2L.** For a set of planar vector forces $\vec{F}_{1},\vec{F}_{2},\vec{F}_{3},\dots,$ acting on a particle, Newton's Second Law says that:
$\sum \vec{F}=m\vec{a}$ 
**Cartesian Coordinates.** If we resolve the forces into their *Cartesian components* and balance the components on each side of this equation, we have:
$\sum \vec{F}=m\vec{a}\implies \sum F_{x}=m\ddot{x},\sum F_{y}=m\ddot{y}$$
**Path Coordinates.** If we resolve the forces into their *path components* and balance the components on each side of this equation, we have:
$\sum \vec{F}=m\vec{a}\implies \sum F_{t}=m\dot{v},\sum F_{n}=m \frac{v^2}{\rho}$$
**Polar Coordinates.** If we resolve the forces into their *polar components* and balance the components on each side of this equation, we have:
$\sum \vec{F}=m\vec{a}\implies \sum F_{r}=m(\ddot{r}-r\dot{\theta}^2),\sum F_{\theta}=m(r \ddot{\theta}+2\dot{r}\dot{\theta})$$

>[!example] Particle P (weighing W) is able to slide within a straight slot cut into an arm. The arm is rotating within a horizontal plane about end $O$ at a constant rate of $\omega$. The slider is being pulled toward $O$ at a constant rate of $\dot{r}$ Determine *(a)* the tension in the cord; *(b)* the normal contact force of the slot on $P$; *(c)* which side of the slot is $P$ in contact with. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=205|figure]]
> *[[Pasted image 20260303210158.png|FBDs]]*
> **Kinetics:**
> $\sum F_{r}=ma_{r}\to-T=\frac{W}{g}a_{r}$$
> $\sum F_{\theta}=ma_{\theta}\to N=\frac{W}{g}a_{\theta}$$
> **Kinematics:**
> $\vec{a}_{p}=\underbrace{ (\dot{r}-r\cancelto{ \omega^2 }{ \dot{\theta}^2 }) }_{ a_{r} }\hat{e}_{r}+\underbrace{ (r \cancel{ \ddot{\theta} }+2\dot{r}\dot{\theta}) }_{ a_{\theta} }\hat{e}_{\theta}$$
> $a_{r}-r\omega^2,a_{\theta}=2\dot{r}\omega$$
> **Solve:**
> $T=\frac{W}{g}(r\omega^2)=2.91\text{lbs}$$
> $N=\frac{W}{g}(2\dot{r}\omega)=-0.777\text{lbs}$$

>[!example] Blocks $A$ and $B$ (having masses of 10kg and 5kg, respectively) are constrained to move along smooth, vertical, and horizontal guides. $A$ and $B$ are connected by a lightweight rod of length $L=2.5\text{m}$. A force of $F=50N$ acts to the right on block $B$. At the position where $s_{A}=1.5\text{m},$ $A$ is moving downward with a speed of $4\text{m/s}$. Determine *(a)* the acceleration of $A$ and $B$ at this instant; *(b)* the force in rod $AB$ at this instant. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=203|figure]]
>*[[Pasted image 20260303211156.png|FBDs]]*
**Kinetics:**
> $\text{A: } \left\{ \begin{matrix}
\sum F_{x}=-N_{A}-\frac{4}{5}F_{AB}=0 \\
\sum F_{y}=-\frac{3}{5}F_{AB}-m_{A}g=m_{A}a_{A}
\end{matrix} \right. $$
> $\text{B: } \left\{ \begin{matrix}
\sum F_{x}=F+\frac{4}{5}F_{AB}=m_{B}a_{B} \\
\sum F_{y}=N_{B}-m_{B}g+\frac{3}{5}F_{AB}=0
\end{matrix} \right.$$
> **Kinematics:**
> $\vec{v}_{A}=\vec{v}_{B}+\vec{\omega}\times \vec{r}_{A/B}\text{ to find }\omega\text{ in terms of }v_{a}$$
> $\vec{a}_{A}=\vec{a}_{B}+\vec{\alpha}\times \vec{r}_{A/B}-\omega^2\vec{r}_{A/B}\text{ to find }\alpha\text{ and }a_{A}\text{ in terms of }a_{B}$$
> $a_{A}=a_{B}\left( \frac{s_{B}}{S_{A}} \right)-\frac{v_{A}^2}{s_{A}}-\frac{v_{A}^2s_{A}}{s_{B}^2}$$
> Could also solve using [[ME 27400/Relative & Constrained Motion\|kinematic constraints]]

>[!example] The system of blocks $A$ and $B$ ($m_{A}=20\text{kg},m_{B}=100\text{kg}$) shown initially at rest when a force $F=60N$ is applied to the free end of the cable. Determine the acceleration of blocks $A$ and $B$ *(a)* if the surface between $A$ and $B$ is smooth; if the surface between $A$ and $B$ is rough with a coefficient of kinetic friction being $\mu_{k}=0.5$, and where it is known that block $A$ slips on block $B$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=201|figure]]
>*[[Pasted image 20260303213138.png|FBDs]]*
>**Kinetics:**
> $\text{A: }\left\{ \begin{matrix}
\sum F_{x}=2F-f_{k}=m_{A}a_{A} \\
\sum F_{y}=N_{1}-m_{A}g=0\to N_{1}=m_{A}g
\end{matrix}  \right.$$
> $\text{B: } \left\{ \begin{matrix}
\sum F_{x}=f_{k}-F=m_{B}a_{B} \\
\sum F_{y}=N_{2}-N_{1}-m_{B}g=0
\end{matrix} \right. $$
> **Solve:**
> $m_{A}a_{A}=2F-\mu_{k}m_{A}g\to a_{A}=\frac{2F}{m}-\mu_{k}g\to \vec{a}_{A}=1.095\text{m/s}^2~ \hat{i}$$
> $m_{B}a_{B}=\mu_{k}m_{A}g-F\to a_{B}=\mu_{k}g\left( \frac{m_{A}}{M_{B}} \right)-\frac{F}{m_{B}}\to \vec{a}_{B}=0.381\text{m/s}^2~\hat{i}$$

>[!example] As a car of mass $m=2000\text{kg}$ braks with a constant braking force $F_{f}=10,000\text{N}$, the speed of the car drops from $v_{1}=80\text{m/s}$ to a speed of $v_{2}=0$ in a distance $s$ and in a time $t$. Determine *(a)* the distance $s$; *(b)* the time $t$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=196|figure]]
>*[[Pasted image 20260303215426.png|FBDs]]*
>**Kinetics:**
> $\begin{matrix}
\sum F_{x}=-F_{f}=ma \\
\sum F_{y}=N-mg=0
\end{matrix}$$
> **Kinematics:**
> $\text{For time, }v(t)\to a=\frac{dv}{dt}$$
> $\text{For distance, }v(s(t))\to a=\frac{dv}{dt}=\frac{dv}{ds}\cdot \frac{ds}{dt}=v \frac{dv}{ds}$$
> **Solve:**
> $-F_{f}=m \frac{dv}{dt}\to \int  _{0} ^t -F_{f}~ d{t}=\int  _{v_{1}} ^0 m~ d{v}\to-F_{f}t=-mv_{1} \text{ so }t=\frac{mv_{1}}{F_{f}}=16\text{s}$$
> $-F_{f}=mv \frac{dv}{ds}\to \int  _{0} ^s -F_{f}~ d{s}=\int  _{v_{1}} ^0 mv~ d{v}\to-F_{f}s=-\frac{1}{2}mv_{1}^2\text{ so }s=\frac{mv_{1}^2}{2F_{f}}=640\text{m}$$

>[!example] A slotted arm rotates about a vertical shaft, passing through $O$ that is at the center of a *fixed* cam. A particle $P$, having a mass $m=0.2kg$ moves within the slot in the arm and remains in contact with the surface of the cam under the action of a spring attached between $P$ and the outer end of the arm. The shape of the cam is such that the radial distance from $O$ to $P$ isgiven by the equation $R=R_{0}-R_{1}\cos(6\theta)$ where $R_{0}=0.5\text{m}$ and $R_{1}=0.1\text{m}$. The spring has a stiffness of $k=500N/m$ and is compressed by an amount $\Delta_{0}=0.2\text{m}$ when $\theta=0$. The arm rotates at a constant rate of $\omega=10\text{rad/s}$. Determine the force acting on $P$ by the cam when $P$ passes over the top of the lobe in the position shown. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=206|figure]]
>*[[Pasted image 20260303220619.png|FBDs]]*
$R_{max}=R_{0}-R_{1}(-1) =R_{0}+R_{1}=0.6\text{m}$$
$R_{min}=R_{0}-R_{1}(1)=0.4\text{m} $$
$F_{sp}=k\cdot\Delta=K(\Delta_{0}+R_{max}-R_{min})=0.4m\cdot K$$
>**Kinetics:**
> 
$\sum F_{r}=N_{2}-F_{sp}=ma_{r} $$
$\sum F_{\theta}=N_{1}=ma_{\theta}$$
> **Kinematics:**
> $\vec{a}_{p}=\underbrace{ (\ddot{r}-\overbrace{ r\dot{\theta}^2 }^{ r\omega^2 }) }_{ a_{r} }\hat{e}_{r}+\underbrace{ (\cancel{ r \ddot{\theta} }+\overbrace{ 2\dot{r}\dot{\theta} }^{ 2\dot{r}\omega }) }_{ a_{\theta} }\hat{e}_{\theta}$$
$r=R_{0}-R_{1}\cos(6\theta) $$
$\dot{r}=R_{1}\sin(6\theta)\overbrace{ (6\dot{\theta}) }^{ 6\omega^2 } $$
$\ddot{r}=R_{1}\cos(6\theta)\underbrace{ (6\dot{\theta})^2 }_{ (6\omega)^2 }+\cancel{ R_{1}\sin(6\theta)(6\ddot{\theta}) }$$
>**Solve:**
> $N_{2}=F_{sp}+ma_{r}=k(0.4\text{m})+m(R_{1}\overbrace{ \cos(6\theta) }^{ -1 }(6\omega)^2)-(R_{0}-R_{1}\overbrace{ \cos(6\theta) }^{ -1 }\omega^2)=-2320\text{N}$$
> 



"Kinetic energy" $T=\frac{1}{2}mv^2$ while "work" $U=\Delta T=\frac{1}{2}m\Delta v^2$ -> *work-energy equation*

Since the work done by a force $\vec{F}$ is the integral of the path projection of the force over the path, we expect that work should be dependent on both the distance traveled & shape of the path. There's a class of forces for which *their work between positions 1 and 2 is independent of the path over which the particles act as it moves from 1 to 2* called "conservative forces" like force due to the action of a spring on a particle and force due to the weight of a particle
$U_{1\to2}=-(V_{2}-V_{1})\text{ where }V=V_{sp}+V_{gr}$$
$V_{sp}=\frac{k}{2}(L-L_{0})^2$$
$V_{gr}=mgh$$
Where $L$ is the current length of the spring, $L_{0}$ is the unstretched length of the spring, and $k$ is the stiffness of the spring. Note that $V_{sp}\geq0$ always. Sign of $V_{gr}$ goes as the sign of $h$ -> if particle is above choice of datum line, $h>0;$ otherwise, $h<0$ 
$U_{1\to2}=U_{1\to2}^{c}+U_{1\to2}^{nc}=-(V_{2}-V_{1})+U^{nc}_{1\to2}$$
$\mathbf{T_{2}+V_{2}=T_{1}+V_{1}+U_{1\to2}^{nc}}$$

>[!example] A block of mass $m=5\text{kg}$ is released from rest on a rough inclined surface w/ $\mu_{k}=0.3$, and slides a distance $d=0.75\text{m}$ toward an uncompressed spring of stiffness $k=1000\text{N/m}$. $\theta=53.13\degree.$ Determine the maximum deflection $\Delta$ of the spring. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=222|figure]]
>*[[Pasted image 20260304111454.png|FBD]]*
>**Kinetics:**
> $T_{1}+V_{1}+U_{1\to2}^{nc}=T_{2}+V_{2},T_{1}=V_{2}=0$$
> $U_{1\to2}^{nc}=\int  _{1}^2 \underbrace{ (\vec{F}\cdot \hat{e}_{t}) }_{ f_{k} }~ d{s}=\int  _{0} ^{d+\Delta}f_{k}~ d{x}=f_{k}(d+\Delta)$$
> $T_{2}=0,V_{2}=-mg(d+\Delta)\sin\theta+\frac{1}{2}k\Delta^2$$
> $\text{so }f_{k}(d+\Delta)=-mg(d+\Delta)\sin\theta+\frac{1}{2}k\Delta^2,\text{ need }f_{k}=\mu_{k}N $$
> $\sum F_{y}=N-mg\cos\theta\to f_{k}=\mu mg\cos\theta$$
> $\dots$$
> $\Delta=0.357\text{m}$$

>[!example] The system shown is made up of particles $A,B,E$ (having masses of 5kg, 20kg, and 80kg, respectively). Lightweight bars $OB$ ($L=0.5\text{m}$) and $OA$ are welded together such that there is a right angle between the two bars, and these bars are welded to the pulley at $O$. Consider the mass of the pulleys to be negligible. The system is released from rest when $\theta=0$ Distance between $OC$ and $r$ is 0.1m. Determine the speed of particle $E$ when $\theta=90\degree$ See [[ME 27400/Dynamics, a Lecturebook.pdf#page=226|figure]].
>*[[Pasted image 20260305163222.png|FBD]]*
>Let the datum be the line going through the midpoint of the pulleys, points $O$ and $C$
>**Kinetics:**
> $T_{1}+V_{1}+U^{nc}_{1\to2}=T_{2}+V_{2} \left\{ \begin{matrix} \\
T_{1}=0 \\
V_{1}=-m_{A}g(2L) \\
U_{1\to2}^{nc}=0 \\
T_{2}=\frac{1}{2}m_{A}v_{A}^2+\frac{1}{2}m_{B}v_{B}^2+\frac{1}{2}m_{E}v_{E}^2 \\
V_{2}=-m_{E}g\Delta E-m_{B}gL \text{ where }\Delta E=r\cdot\theta
\end{matrix} \right.$$
> **Kinematics** (need $v_{A},v_{B},v_{E}$)
> $v_{A}=\omega_{O}2L$$
> $v_{B}=\omega_{O}L$$
> $v_{E}=\frac{d}{dt}(r\theta)=r\dot{\theta}=\omega_{O}r$$
> **Solve**
> $-m_{A}g(2L)=2m_{A}\omega_{O}^2L^2+\frac{1}{2}m_{B}\omega_{O}^2L^2+\frac{1}{2}m_{E}\omega_{O}^2r^2-m_{E}gr\theta-m_{B}gL$$
> $\omega_{O}=\sqrt{ \frac{g\left( m_{E}r \frac{\pi}{2}+m_{B}L-2m_{A}L \right)}{2m_{A}L^2+\frac{1}{2}m_{B}L^2+\frac{1}{2}m_{E}r^2 }}=5.65\text{rad/s}$$
> $v_{E}=\omega_{O}r=0.565\text{m/s}$$

>[!example] Block $A$, having a mass of $m=5\text{kg}$, is able to slide within a smooth, inclined slot. A spring of stiffness $k=50\text{N/m}$ is attached between $A$ and a fixed point at $O$, as shown in the figure. A constant horizontal force $F=300\text{N}$ acts on the block. The system is released from rest at position 1, where at position 1, the spring $\perp$ slot and is unstretched. At position 2, block $A$ is directly above $O$. Additionally, $\theta=53.13\degree$ and $d=0.2\text{m}$. Assuming that block $A$ reaches position $2$, determine the speed of $A$ at position 2. If $A$ does not reach position 2, explain why not. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=228|figure]]
>*[[Pasted image 20260305171955.png|FBD]]*
>**Kinetics:**
> $T_{1}+V_{1}+U^{nc}_{1\to2}=T_{2}+V_{2} \left\{ \begin{matrix}
T_{1}=0 \\
V_{1}=0
\end{matrix}\right.$$
> $U_{1\to2}^{nc}=\int  _{1}^2 (\vec{F}\cdot \hat{e}_{t})~ d{s}=\int  _{1}^2 F\hat{i}\cdot(dx \hat{i}+dy \hat{j})=\int  _{0} ^{d\cos\theta}F~ d{x}=Fd\cos\theta$$
> $T_{2}=\frac{1}{2}m_{2}v_{2}^2$$
> $v_{2}=mgd\sin\theta+\frac{1}{2}K\Delta^2\text{ where }\Delta=L-L_{0} \left\{ \begin{matrix}
L_{0}=\frac{d}{\tan\theta} \\
L=\sqrt{ L_{0}^2+d^2 }
\end{matrix} \right.$$
**Solve**
> $U_{1\to2}^{nc}=T_{2}+V_{2}$$
> $\dots v=3.34\text{m/s}$ 




# Linear Impulse-Momentum Equation for a Single Particle
$m\vec{v}_{2}=m\vec{v}_{1}+\int  _{1}^2 \vec{R}~ d{t}$$
where $m\vec{v}$ is the *linear momentum* of the particle and $\int _1^2\vec{R}~ d{t}$ is the *impulse* of the net force acting on the particle
1. The above is the impulse-momentum equation for a particle since the equation relates the change in laer momentum to the impulse acting on the particle
2. Note that this equation relates the change in velocity of the particle to a change in time (from $t=t_{1}$ to $t=t_{2}$)
3. In contrast with the work-energy equation, the impulse-momentum is a vector equation, that is, the equation can be resolved into components. For example, if the forces acting on the particle are resolved into a set of $x-y$ Cartesian components, then the above vector equation represents the following two sets of scalar equations:
$mv_{x2}=mv_{x1}+\int  _{1}^2 R_{x}~ d{t}$$
$mv_{y2}=mv_{y1}+\int  _{1}^2 R_{y}~ d{t}$$
4. If the resultant force in a given diretion is zero, then linaer momentum is *conserved* in that direction. For example, suppose that $R_{x}=0;$ then from above we see that:
$mv_{x2}=mv_{x2}\implies v_{x2}=v_{x1}$$
Conservation of momentum in one direction does not imply conservation in any other directions
5. *Conservation of momentum does not imply or result from conservation of energy.* Momentum and energy are two independent quantities
# Impulse-Momentum Equation for a System of Particles
$\sum m_{j}\vec{v}_{j2}=\sum m_{j}\vec{v}_{j1}+\int  _{1} ^2 \left[ \sum \vec{F}_{j}^{ext} \right]~ d{t}$$
where $\sum m_{j}\vec{v}_{j}$ is the total linear momentum of the system and $\sum \vec{F}_{j}^{ext}$ is the resultant external force acting on the $j$th particle
1. Recall that the above equation results from the summation of impulse-momentum equation for each particle in the system. An important result of this is that *internal* forces cancel, and the impulse due to only the *external* forces contributes to the change of the total linear momentum of the system
2. It is advisable to make your choice of the system to be as large as possibly to make as many forces *internal* to the system as possible. However, remember than any force that is internal to the system cannot be determined from this equation
3. As before, note that the linear impulse-momentum equation is a vector equation
4. Linear momentum for a system, in a given direction, is conserved when the net external forces in that direction is zero. When working problems with the impulse-momentum equations, draw the FBD of your system: look for directions in which there are no net forces. In these directions, you can use conservation of linear momentum

>[!example] A tug having a mass of $m$ is towing a coal barge (mass $M$) with a speed of $v_{A1}$. During a short period of time $\Delta t$ whne the engines of the tug are turned off, the stern wenchtakes in the towing cable at a rate of $v_{B/A}$. Determine (a) the speed of the tug during this time; (b) the average value of the tension in the towing cable during this time. Ignore water resistance on the tug and barge, also assume that the towing cable remains taut at all times. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=240|figure]]
>*[[Pasted image 20260305184829.png|FBD (a)]], [[Pasted image 20260305190103.png|FBD (b)]]*
>**Kinetics:**
> $\text{Since }\sum F_{x}=0,\text{ linear momentum is conserved in }x\text{-direction}$$
> $mv_{A1}+mv_{B1}+\int  _{1}^2 \cancel{ F_{x} } d{t}=mv_{A2}+mv_{B2}$$
> $v_{A1}=v_{B1}\text{ so }(m+M)v_{A1}=mv_{A2}+mv_{B2}$$
> $v_{B2}=v_{A2}+v_{B/A}\to (m+M)v_{A1}=(m+M)v_{A2}+mv_{B/A}$$
> $\text{(a) }\textcolor{green}{v_{A2}=v_{A1}-\frac{m}{M+m}v_{B/A}}$$
> $\text{In x-direction: }mv_{A1}+\int  _{1}^2 T~ d{t}=mv_{A2}\to mv_{A1}+T\Delta t=mv_{A2}$$
> $\text{(b) } \textcolor{green}{T=\frac{m(v_{A2}-v_{A1})}{\Delta t}}$$

>[!example] Block $P$, weighing 100lb, is initially stationary when a force $F(t)$ begins acting on it, with $F(t)$ given in the graph shown. The coefficients of static and kinetic friction between the block and horizontal surface on which it moves are known to be $\mu_{s}=0.5,\mu_{k}=0.2$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=239|figures]]
>*[[Pasted image 20260305190612.png|FBD]]*
>**Kinetics:**
>$F_{s,max}=\mu_{s}N=\mu_{s}W=50\text{lb},\text{ since }F(t)=20t,f_{s}\text{ is maximized at }t=2.5\text{s}$$
> $\text{in }x\text{-direction: }mv_{1}+\int  _{1}^2 (F-f)~ d{t}=mv_{2}$$
> $\text{When does the block begin to move? }F_{s,max}=\mu_{s}N;\sum F_{y}=N-W=0\text{ so }F_{s,max}=\mu_{s}W=50\text{lb}$$
> $\cancel{ mv_{1} }+\int  _{2.5\text{s}} ^{10\text{s}} \left( 20\frac{\text{lb}}{\text{s}} -\mu_{k}W\right)~ d{t}=mv_{2}$$
> $\left. 10 \frac{\text{lb}}{\text{s}}\cdot t^2-20\text{lb}\cdot t~ \right|^{10\text{s}} _{2.5\text{s}}=787.5\text{lb}\cdot\text{s}$$
> $m=\frac{W}{g},m=3.11 \frac{\text{lb}\cdot s^2}{\text{ft}}\to \textcolor{green}{v_{2}=253.4\text{ft/s}}$$

