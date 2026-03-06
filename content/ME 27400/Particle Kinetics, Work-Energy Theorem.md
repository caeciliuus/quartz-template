---
publish: true
created: 2026-03-05T17:27:14.158-05:00
modified: 2026-03-05T20:02:22.671-05:00
tags:
  - S2
  - lecture
  - me274
cssclasses: ""
---

"Kinetic energy" $T=\frac{1}{2}mv^2$ while "work" $U=\Delta T=\frac{1}{2}m\Delta v^2$ -> *work-energy equation*

Since the work done by a force $\vec{F}$ is the integral of the path projection of the force over the path, we expect that work should be dependent on both the distance traveled & shape of the path. There's a class of forces for which *their work between positions 1 and 2 is independent of the path over which the particles act as it moves from 1 to 2* called "conservative forces" like force due to the action of a spring on a particle and force due to the weight of a particle
$$U_{1\to2}=-(V_{2}-V_{1})\text{ where }V=V_{sp}+V_{gr}$$
$$V_{sp}=\frac{k}{2}(L-L_{0})^2$$
$$V_{gr}=mgh$$
Where $L$ is the current length of the spring, $L_{0}$ is the unstretched length of the spring, and $k$ is the stiffness of the spring. Note that $V_{sp}\geq0$ always. Sign of $V_{gr}$ goes as the sign of $h$ -> if particle is above choice of datum line, $h>0;$ otherwise, $h<0$ 
$$U_{1\to2}=U_{1\to2}^{c}+U_{1\to2}^{nc}=-(V_{2}-V_{1})+U^{nc}_{1\to2}$$
$$\mathbf{T_{2}+V_{2}=T_{1}+V_{1}+U_{1\to2}^{nc}}$$

>[!example] A block of mass $m=5\text{kg}$ is released from rest on a rough inclined surface w/ $\mu_{k}=0.3$, and slides a distance $d=0.75\text{m}$ toward an uncompressed spring of stiffness $k=1000\text{N/m}$. $\theta=53.13\degree.$ Determine the maximum deflection $\Delta$ of the spring. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=222|figure]]
>*[[Pasted image 20260304111454.png|FBD]]*
>**Kinetics:**
> $$T_{1}+V_{1}+U_{1\to2}^{nc}=T_{2}+V_{2},T_{1}=V_{2}=0$$
> $$U_{1\to2}^{nc}=\int  _{1}^2 \underbrace{ (\vec{F}\cdot \hat{e}_{t}) }_{ f_{k} }~ d{s}=\int  _{0} ^{d+\Delta}f_{k}~ d{x}=f_{k}(d+\Delta)$$
> $$T_{2}=0,V_{2}=-mg(d+\Delta)\sin\theta+\frac{1}{2}k\Delta^2$$
> $$\text{so }f_{k}(d+\Delta)=-mg(d+\Delta)\sin\theta+\frac{1}{2}k\Delta^2,\text{ need }f_{k}=\mu_{k}N $$
> $$\sum F_{y}=N-mg\cos\theta\to f_{k}=\mu mg\cos\theta$$
> $$\dots$$
> $$\Delta=0.357\text{m}$$

>[!example] The system shown is made up of particles $A,B,E$ (having masses of 5kg, 20kg, and 80kg, respectively). Lightweight bars $OB$ ($L=0.5\text{m}$) and $OA$ are welded together such that there is a right angle between the two bars, and these bars are welded to the pulley at $O$. Consider the mass of the pulleys to be negligible. The system is released from rest when $\theta=0$ Distance between $OC$ and $r$ is 0.1m. Determine the speed of particle $E$ when $\theta=90\degree$ See [[ME 27400/Dynamics, a Lecturebook.pdf#page=226|figure]].
>*[[Pasted image 20260305163222.png|FBD]]*
>Let the datum be the line going through the midpoint of the pulleys, points $O$ and $C$
>**Kinetics:**
> $$T_{1}+V_{1}+U^{nc}_{1\to2}=T_{2}+V_{2} \left\{ \begin{matrix} \\
T_{1}=0 \\
V_{1}=-m_{A}g(2L) \\
U_{1\to2}^{nc}=0 \\
T_{2}=\frac{1}{2}m_{A}v_{A}^2+\frac{1}{2}m_{B}v_{B}^2+\frac{1}{2}m_{E}v_{E}^2 \\
V_{2}=-m_{E}g\Delta E-m_{B}gL \text{ where }\Delta E=r\cdot\theta
\end{matrix} \right.$$
> **Kinematics** (need $v_{A},v_{B},v_{E}$)
> $$v_{A}=\omega_{O}2L$$
> $$v_{B}=\omega_{O}L$$
> $$v_{E}=\frac{d}{dt}(r\theta)=r\dot{\theta}=\omega_{O}r$$
> **Solve**
> $$-m_{A}g(2L)=2m_{A}\omega_{O}^2L^2+\frac{1}{2}m_{B}\omega_{O}^2L^2+\frac{1}{2}m_{E}\omega_{O}^2r^2-m_{E}gr\theta-m_{B}gL$$
> $$\omega_{O}=\sqrt{ \frac{g\left( m_{E}r \frac{\pi}{2}+m_{B}L-2m_{A}L \right)}{2m_{A}L^2+\frac{1}{2}m_{B}L^2+\frac{1}{2}m_{E}r^2 }}=5.65\text{rad/s}$$
> $$v_{E}=\omega_{O}r=0.565\text{m/s}$$

>[!example] Block $A$, having a mass of $m=5\text{kg}$, is able to slide within a smooth, inclined slot. A spring of stiffness $k=50\text{N/m}$ is attached between $A$ and a fixed point at $O$, as shown in the figure. A constant horizontal force $F=300\text{N}$ acts on the block. The system is released from rest at position 1, where at position 1, the spring $\perp$ slot and is unstretched. At position 2, block $A$ is directly above $O$. Additionally, $\theta=53.13\degree$ and $d=0.2\text{m}$. Assuming that block $A$ reaches position $2$, determine the speed of $A$ at position 2. If $A$ does not reach position 2, explain why not. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=228|figure]]
>*[[Pasted image 20260305171955.png|FBD]]*
>**Kinetics:**
> $$T_{1}+V_{1}+U^{nc}_{1\to2}=T_{2}+V_{2} \left\{ \begin{matrix}
T_{1}=0 \\
V_{1}=0
\end{matrix}\right.$$
> $$U_{1\to2}^{nc}=\int  _{1}^2 (\vec{F}\cdot \hat{e}_{t})~ d{s}=\int  _{1}^2 F\hat{i}\cdot(dx \hat{i}+dy \hat{j})=\int  _{0} ^{d\cos\theta}F~ d{x}=Fd\cos\theta$$
> $$T_{2}=\frac{1}{2}m_{2}v_{2}^2$$
> $$v_{2}=mgd\sin\theta+\frac{1}{2}K\Delta^2\text{ where }\Delta=L-L_{0} \left\{ \begin{matrix}
L_{0}=\frac{d}{\tan\theta} \\
L=\sqrt{ L_{0}^2+d^2 }
\end{matrix} \right.$$
**Solve**
> $$U_{1\to2}^{nc}=T_{2}+V_{2}$$
> $$\dots v=3.34\text{m/s}$$ 

