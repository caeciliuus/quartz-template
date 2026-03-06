---
publish: true
created: 2026-01-28T14:27:59.110-05:00
modified: 2026-03-05T20:22:26.721-05:00
tags:
  - S2
  - lecture
  - me274
cssclasses: ""
---

# ![[Attachments/Pasted image 20260128143709.png|right|200]] Relative Motion
- By definition, $\vec{r}_{B/A}$ is the vector pointing FROM point A TO point B -> $\vec{r}_{B/A}=\vec{r}_{B}-\vec{r}_{A}$
- Taking derivatives we get 
$$\frac{d}{dt} \vec{r}_{B/A}=\frac{d}{dt}\vec{r}_{B}-\frac{d}{dt}\vec{r}_{A}\to \vec{v}_{B/A}=\vec{v}_{B}-\vec{v}_{A}$$
$$\frac{d^2}{dt^2}\vec{r}_{B/A}=\frac{d^2}{dt^2}\vec{r}_{B}-\frac{d^2}{dt^2}\vec{r}_{A}\to \vec{a}_{{B/A}}=\vec{a}_{B}-\vec{a}_{A}$$

>[!example] Jet B traveling due north w/ speed of $v_{B}=600km/hr$. Passengers on jet $B$ observe $A$ to be flying sideways and motive due east. Determine *(a)* the speed of $A$; *(b)* the speed of $A$ as observed by the passengers on jet $B$. *[[ME 27400/Dynamics, a Lecturebook.pdf#page=64|Dynamics, a Lecturebook, page 64]]* 
> $$\vec{v}_{A/B}=\vec{v}_{A}-\vec{v}_{B}=?\hat{i}+0\hat{j}$$
> $$\vec{v}_{A}-\vec{v}_{B}=(\dot{x} _{A}\hat{i}+\dot{y}_{A} \hat{j})-(\dot{x}_{B} \hat{i}+\dot{y}_{B} \hat{j})=(\dot{x}_{A}-\dot{x}_{B})\hat{i}+\cancel{ (\dot{y}_{A}-\dot{y}_{B}) }\hat{j} ~[\dot{y}_{A}=\dot{y}_{B}=v_{B}]$$
> $$v_{A}\sin30=600km/hr\to v_{A}=1200 km/hr$$
> $$\vec{v}_{A/B}=(\dot{x}_{A}-\cancel{ \dot{x}_{B} })\hat{i}=v_{A}\cos30 \hat{i}=1039km/hr$$
# Constrained Motion
The above expressions relate the general motion of two points A & B. Often, their relative motion is constrained so that one point's motion depends on the other's. One [[ME 27400/Dynamics, a Lecturebook.pdf#page=60|example]] of this is when a taut, inextensible cable connects the two points
- Since the cable is inextensible, the length $L$ of the cable does not change as the positions of points $A$ and $B$ change.
- Since a cable is flexible, it can be pulled over a pulley, as shown above right. Since the cable is inextensible, $L$ remains constant for all motion of $A$ and $B$ so long as the cable remains taut. The distance between ends A and B does not, however, remain constant
Based on these remarks, we can set up some general steps for solving problems for which particles are connected by taut, inextensible cables
1. Carefully define set of coordinates that describe the motion of the various particles in the system
2. For each cable, write an expression for its length $L$ in terms of an appropriate set of coordinates defined in step 1
3. Differentiate w.r.t time the expression for $L$ and set $\frac{dL}{dt}=0$ to determine velocity constant
4. Repeat steps 2 - 4 for each cable in the system

> [!example] Block $B$ has a constant acceleration of $a_{B}=3 m/s^2$ to the right. At the instant shown, $B$ has a velocity of $2m/s$ to the right. Determine *(a)* the velocity of block $A$; *(b)* the acceleration of block $A$ (See [[ME 27400/Dynamics, a Lecturebook.pdf#page=65|Dynamics, a Lecturebook, page 65]])
> First find a zero-point to pull cables against. Pulleys move w/ block so define datum relative to something unmoving. In this case it'll be the right side of the small wall at the bottom. 
> $$L=4x_{A}+3x_{B}$$
> $$\frac{dL}{dt}=0=4\dot{x}_{A}+3\dot{x}_{B}\to4\dot{x}_{A}=-3\dot{x}_{B}\to \dot{x}_{A}=-\frac{3}{4}\dot{x}_{B}=-1.5m/s$$
> $$\frac{d^2L}{dt^2}=0=4\ddot{x}_{A}+3\ddot{x}_{B}\to \ddot{x}_{A}=-\frac{3}{4}\ddot{x}_{B}=-2.25m/s^2$$

# Examples
>[!example] End $B$ of the link moves to the right with a constant speed $v_{B}$. Determine $(a)$ the angular velocity of link $AB$; and $(b)$ the angular acceleration of link $AB$ (See [[ME 27400/Dynamics, a Lecturebook.pdf#page=101|Dynamics, a Lecturebook, page 101]])
>$$\vec{v}_{A}=\vec{v}_{B}+\vec{\omega}\times \vec{r}_{A/B},\vec{r}_{A/B}=L(-\cos\theta \hat{i}+\sin\theta \hat{j})$$
> $$-v_{A}\hat{j}=\vec{v}_{B}+\omega \hat{k}\times(-L\cos\theta \hat{i}+L\sin\theta \hat{j})=v_{B}\hat{i}-\omega L\cos\theta \hat{j}-wL\sin\theta \hat{i}$$
> $$0=v_{B}-wL\sin\theta,\omega=\frac{v_{B}}{L\sin\theta}=10\hat{k}~rad/s$$
> $$\vec{a}_{A}=\cancel{ \vec{a}_{B}}+\vec{\alpha} \times \vec{r}_{B/A}-\omega^2 \vec{r}_{B/A}$$
> $$-a_{A}\hat{j}=\alpha \hat{k}\times(-L\cos\theta \hat{i}+L\sin\theta \hat{j})-\left[ \left( \frac{v_{B}}{L\sin\theta} \right)^2(-L\cos\theta \hat{i})+L\sin\theta \hat{j} \right]$$
> $$=-L\alpha \cos\theta \hat{j}-L\alpha \sin\theta \hat{i}+\frac{v_{B}^2\cos\theta}{L\sin^2\theta}\hat{i}-\frac{v_{B}^2}{L\sin\theta}\hat{j}$$
> $$\hat{i}:0=-L\alpha \sin\theta+\frac{v_{B}^2\cos\theta}{L\sin^2\theta}\to L\alpha \sin\theta=\frac{v_{B}^2\cos\theta}{L\sin^2\theta},\alpha=\frac{v_{b}^2\cos\theta}{L^2\sin^3\theta}=133.33\hat{k}~rad/s^2$$