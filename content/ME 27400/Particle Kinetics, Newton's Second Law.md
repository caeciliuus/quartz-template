---
publish: true
created: 2026-03-05T17:28:31.258-05:00
modified: 2026-03-05T20:02:22.663-05:00
tags:
  - S2
  - lecture
  - me274
cssclasses: ""
---

**N2L.** For a set of planar vector forces $\vec{F}_{1},\vec{F}_{2},\vec{F}_{3},\dots,$ acting on a particle, Newton's Second Law says that:
$$\sum \vec{F}=m\vec{a}$$ 
**Cartesian Coordinates.** If we resolve the forces into their *Cartesian components* and balance the components on each side of this equation, we have:
$$\sum \vec{F}=m\vec{a}\implies \sum F_{x}=m\ddot{x},\sum F_{y}=m\ddot{y}$$
**Path Coordinates.** If we resolve the forces into their *path components* and balance the components on each side of this equation, we have:
$$\sum \vec{F}=m\vec{a}\implies \sum F_{t}=m\dot{v},\sum F_{n}=m \frac{v^2}{\rho}$$
**Polar Coordinates.** If we resolve the forces into their *polar components* and balance the components on each side of this equation, we have:
$$\sum \vec{F}=m\vec{a}\implies \sum F_{r}=m(\ddot{r}-r\dot{\theta}^2),\sum F_{\theta}=m(r \ddot{\theta}+2\dot{r}\dot{\theta})$$

>[!example] Particle P (weighing W) is able to slide within a straight slot cut into an arm. The arm is rotating within a horizontal plane about end $O$ at a constant rate of $\omega$. The slider is being pulled toward $O$ at a constant rate of $\dot{r}$ Determine *(a)* the tension in the cord; *(b)* the normal contact force of the slot on $P$; *(c)* which side of the slot is $P$ in contact with. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=205|figure]]
> *[[Pasted image 20260303210158.png|FBDs]]*
> **Kinetics:**
> $$\sum F_{r}=ma_{r}\to-T=\frac{W}{g}a_{r}$$
> $$\sum F_{\theta}=ma_{\theta}\to N=\frac{W}{g}a_{\theta}$$
> **Kinematics:**
> $$\vec{a}_{p}=\underbrace{ (\dot{r}-r\cancelto{ \omega^2 }{ \dot{\theta}^2 }) }_{ a_{r} }\hat{e}_{r}+\underbrace{ (r \cancel{ \ddot{\theta} }+2\dot{r}\dot{\theta}) }_{ a_{\theta} }\hat{e}_{\theta}$$
> $$a_{r}-r\omega^2,a_{\theta}=2\dot{r}\omega$$
> **Solve:**
> $$T=\frac{W}{g}(r\omega^2)=2.91\text{lbs}$$
> $$N=\frac{W}{g}(2\dot{r}\omega)=-0.777\text{lbs}$$

>[!example] Blocks $A$ and $B$ (having masses of 10kg and 5kg, respectively) are constrained to move along smooth, vertical, and horizontal guides. $A$ and $B$ are connected by a lightweight rod of length $L=2.5\text{m}$. A force of $F=50N$ acts to the right on block $B$. At the position where $s_{A}=1.5\text{m},$ $A$ is moving downward with a speed of $4\text{m/s}$. Determine *(a)* the acceleration of $A$ and $B$ at this instant; *(b)* the force in rod $AB$ at this instant. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=203|figure]]
>*[[Pasted image 20260303211156.png|FBDs]]*
**Kinetics:**
> $$\text{A: } \left\{ \begin{matrix}
\sum F_{x}=-N_{A}-\frac{4}{5}F_{AB}=0 \\
\sum F_{y}=-\frac{3}{5}F_{AB}-m_{A}g=m_{A}a_{A}
\end{matrix} \right. $$
> $$\text{B: } \left\{ \begin{matrix}
\sum F_{x}=F+\frac{4}{5}F_{AB}=m_{B}a_{B} \\
\sum F_{y}=N_{B}-m_{B}g+\frac{3}{5}F_{AB}=0
\end{matrix} \right.$$
> **Kinematics:**
> $$\vec{v}_{A}=\vec{v}_{B}+\vec{\omega}\times \vec{r}_{A/B}\text{ to find }\omega\text{ in terms of }v_{a}$$
> $$\vec{a}_{A}=\vec{a}_{B}+\vec{\alpha}\times \vec{r}_{A/B}-\omega^2\vec{r}_{A/B}\text{ to find }\alpha\text{ and }a_{A}\text{ in terms of }a_{B}$$
> $$a_{A}=a_{B}\left( \frac{s_{B}}{S_{A}} \right)-\frac{v_{A}^2}{s_{A}}-\frac{v_{A}^2s_{A}}{s_{B}^2}$$
> Could also solve using [[ME 27400/Relative & Constrained Motion\|kinematic constraints]]

>[!example] The system of blocks $A$ and $B$ ($m_{A}=20\text{kg},m_{B}=100\text{kg}$) shown initially at rest when a force $F=60N$ is applied to the free end of the cable. Determine the acceleration of blocks $A$ and $B$ *(a)* if the surface between $A$ and $B$ is smooth; if the surface between $A$ and $B$ is rough with a coefficient of kinetic friction being $\mu_{k}=0.5$, and where it is known that block $A$ slips on block $B$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=201|figure]]
>*[[Pasted image 20260303213138.png|FBDs]]*
>**Kinetics:**
> $$\text{A: }\left\{ \begin{matrix}
\sum F_{x}=2F-f_{k}=m_{A}a_{A} \\
\sum F_{y}=N_{1}-m_{A}g=0\to N_{1}=m_{A}g
\end{matrix}  \right.$$
> $$\text{B: } \left\{ \begin{matrix}
\sum F_{x}=f_{k}-F=m_{B}a_{B} \\
\sum F_{y}=N_{2}-N_{1}-m_{B}g=0
\end{matrix} \right. $$
> **Solve:**
> $$m_{A}a_{A}=2F-\mu_{k}m_{A}g\to a_{A}=\frac{2F}{m}-\mu_{k}g\to \vec{a}_{A}=1.095\text{m/s}^2~ \hat{i}$$
> $$m_{B}a_{B}=\mu_{k}m_{A}g-F\to a_{B}=\mu_{k}g\left( \frac{m_{A}}{M_{B}} \right)-\frac{F}{m_{B}}\to \vec{a}_{B}=0.381\text{m/s}^2~\hat{i}$$

>[!example] As a car of mass $m=2000\text{kg}$ braks with a constant braking force $F_{f}=10,000\text{N}$, the speed of the car drops from $v_{1}=80\text{m/s}$ to a speed of $v_{2}=0$ in a distance $s$ and in a time $t$. Determine *(a)* the distance $s$; *(b)* the time $t$. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=196|figure]]
>*[[Pasted image 20260303215426.png|FBDs]]*
>**Kinetics:**
> $$\begin{matrix}
\sum F_{x}=-F_{f}=ma \\
\sum F_{y}=N-mg=0
\end{matrix}$$
> **Kinematics:**
> $$\text{For time, }v(t)\to a=\frac{dv}{dt}$$
> $$\text{For distance, }v(s(t))\to a=\frac{dv}{dt}=\frac{dv}{ds}\cdot \frac{ds}{dt}=v \frac{dv}{ds}$$
> **Solve:**
> $$-F_{f}=m \frac{dv}{dt}\to \int  _{0} ^t -F_{f}~ d{t}=\int  _{v_{1}} ^0 m~ d{v}\to-F_{f}t=-mv_{1} \text{ so }t=\frac{mv_{1}}{F_{f}}=16\text{s}$$
> $$-F_{f}=mv \frac{dv}{ds}\to \int  _{0} ^s -F_{f}~ d{s}=\int  _{v_{1}} ^0 mv~ d{v}\to-F_{f}s=-\frac{1}{2}mv_{1}^2\text{ so }s=\frac{mv_{1}^2}{2F_{f}}=640\text{m}$$

>[!example] A slotted arm rotates about a vertical shaft, passing through $O$ that is at the center of a *fixed* cam. A particle $P$, having a mass $m=0.2kg$ moves within the slot in the arm and remains in contact with the surface of the cam under the action of a spring attached between $P$ and the outer end of the arm. The shape of the cam is such that the radial distance from $O$ to $P$ isgiven by the equation $R=R_{0}-R_{1}\cos(6\theta)$ where $R_{0}=0.5\text{m}$ and $R_{1}=0.1\text{m}$. The spring has a stiffness of $k=500N/m$ and is compressed by an amount $\Delta_{0}=0.2\text{m}$ when $\theta=0$. The arm rotates at a constant rate of $\omega=10\text{rad/s}$. Determine the force acting on $P$ by the cam when $P$ passes over the top of the lobe in the position shown. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=206|figure]]
>*[[Pasted image 20260303220619.png|FBDs]]*
$$R_{max}=R_{0}-R_{1}(-1) =R_{0}+R_{1}=0.6\text{m}$$
$$R_{min}=R_{0}-R_{1}(1)=0.4\text{m} $$
$$F_{sp}=k\cdot\Delta=K(\Delta_{0}+R_{max}-R_{min})=0.4m\cdot K$$
>**Kinetics:**
> 
$$\sum F_{r}=N_{2}-F_{sp}=ma_{r} $$
$$\sum F_{\theta}=N_{1}=ma_{\theta}$$
> **Kinematics:**
> $$\vec{a}_{p}=\underbrace{ (\ddot{r}-\overbrace{ r\dot{\theta}^2 }^{ r\omega^2 }) }_{ a_{r} }\hat{e}_{r}+\underbrace{ (\cancel{ r \ddot{\theta} }+\overbrace{ 2\dot{r}\dot{\theta} }^{ 2\dot{r}\omega }) }_{ a_{\theta} }\hat{e}_{\theta}$$
$$r=R_{0}-R_{1}\cos(6\theta) $$
$$\dot{r}=R_{1}\sin(6\theta)\overbrace{ (6\dot{\theta}) }^{ 6\omega^2 } $$
$$\ddot{r}=R_{1}\cos(6\theta)\underbrace{ (6\dot{\theta})^2 }_{ (6\omega)^2 }+\cancel{ R_{1}\sin(6\theta)(6\ddot{\theta}) }$$
>**Solve:**
> $$N_{2}=F_{sp}+ma_{r}=k(0.4\text{m})+m(R_{1}\overbrace{ \cos(6\theta) }^{ -1 }(6\omega)^2)-(R_{0}-R_{1}\overbrace{ \cos(6\theta) }^{ -1 }\omega^2)=-2320\text{N}$$
> 
