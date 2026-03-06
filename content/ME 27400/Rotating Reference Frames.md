---
publish: true
created: 2026-03-02T20:52:27.442-05:00
modified: 2026-03-05T20:02:22.707-05:00
tags:
  - S2
  - lecture
  - me274
cssclasses: ""
---

# Rotating Reference Frame Kinematics [2D]
$$\vec{v}_{B}=\vec{v}_{A}+(\vec{v}_{B/A})_{rel}+\vec{\omega}\times \vec{r}_{B/A}=\vec{v}_{A}+\vec{v}_{B/A}$$
$$\vec{a}_{B}=\vec{a}_{A}+(\vec{a}_{B/A})_{rel}+\vec{\alpha}\times \vec{r}_{B/A}+2\vec{\omega}\times(\vec{v}_{B/A})+\vec{\omega}\times[\vec{\omega}\times \vec{r}_{B/A}]=\vec{a}_{A}+\vec{a}_{B/A}$$
- $\vec{v}_{A}$ and $\vec{v}_{B}$ are the velocities of points $B$ and $A$ as seen by a fixed observer 
- $\vec{a}_{A}$ and $\vec{a}_{B}$ are the accelerations of points $B$ and $A$ as seen by a fixed observer
- $\vec{\omega}$ is angular velocity of the moving observer
- $\vec{\alpha}$ is the angular acceleration of the moving observer
- $(\vec{v}_{B/A})_{rel}/(\vec{a}_{B/A})_{rel}$ is the "velocity/acceleration of point $B$ as seen by the moving observer at $A$". In order to write down this term, you must clearly understand how the moving observer views the motion of $B$
- The term $2\vec{\omega}\times(\vec{v}_{B/A})_{rel}$ is known as the "Coriolis" component of acceleration. The term arises due to an observed velocity of $B$ by the moving observer, when the observer has a non-zero angular velocity

>[!question] What are the differences between $\vec{v}_{B/A}$ and $(\vec{v}_{B/A})_{rel}?$ And between $\vec{a}_{B/A}$ and $(\vec{a}_{B/A})_{rel}?$ Are they ever the same?
> $$(\vec{v}_{B/A})_{rel}=\vec{v}_{B/A}-\vec{\omega}\times r_{B/A}$$
> $$(\vec{a}_{B/A})_{rel}=\vec{a}_{B/A}-\vec{\alpha}\times \vec{r}_{B/A}-2\vec{\omega}\times(\vec{v}_{B/A})_{rel}-\vec{\omega}[\vec{\omega}\times \vec{r}_{B/A}]$$
> We see that if the observer is translating but not rotating (i.e. $\vec{\omega}=\vec{\alpha}=0$), then $(\vec{v}_{B/A})_{rel}=\vec{v}_{B/A}$ and $(\vec{a}_{B/A})_{rel}=\vec{a}_{B/A}$. The rotational terms on the RHS of the above equations provide us with information on how the motion of $B$ as seen by the observer is distorted by the rotation of the observer 

>[!example] The disk rolls without slipping to the right with a *constant* angular speed of $\omega_{d}.$ At the instant shown, pin $P$ is directly above the center $A$ of the disk. Determine *(a)* the angular acceleration of the disk; *(b)* the acceleration of $P$ as seen by an observer on arm $BD$. $\omega_{d}=20rad/s,x_{a}=0.48m,r=0.14m,R=0.2m.$ See [[ME 27400/Dynamics, a Lecturebook.pdf#page=159|figure]]
> $$\vec{\alpha}_{d}=0, (\vec{v}_{p/b})_{rel}=\dot{x}_{A}\hat{i} (\vec{a}_{p/b})_{rel}=\ddot{x}_{A}\hat{i}$$
> $$\vec{a}_{p}=\cancel{ \vec{a}_{B} }+(a_{p/b})_{rel}+\vec{\alpha}_{BD}\times \vec{r}_{P/B}+2\vec{\omega}_{BD}\times(\vec{v}_{p/B})_{rel}-\omega^2_{BD}\vec{r}_{P/B}$$
> $$\vec{a}_{p}=\ddot{x}_{A}\hat{i}+(\alpha_{BD}\hat{k})\times(\alpha_{A}\hat{i})+(2\omega_{BD}\hat{k}\times(\dot{x}_{A}\hat{i}))-\omega^2_{BD}(x_{A}\hat{i})$$
> $$\vec{v}_{p}=\cancel{ \vec{v}_{B} }+(\vec{v}_{p/b})_{rel}+\vec{\omega}_{BD}\times \vec{r}_{p/B}=\dot{x}_{A}\hat{i}+(\omega_{BD}\hat{k})\times(x_{A}\hat{i})=\dot{x}_{A}\hat{i}+\omega_{BD}x_{A}\hat{j}$$
> $$\vec{v}_{p}=\cancel{ \vec{v}_{c} }+\vec{\omega}_{d}\times \vec{r}_{p/c}=(-\omega_{d}\hat{k})\times(R+r \hat{j})=\omega_{d}(R+r)\hat{I}\text{ where }\hat{I}=\cos\theta \hat{i}-\sin\theta \hat{j}$$
> $$\to \vec{v}_{P}=\omega_{d}(R+r)\hat{I}$$
> $$\omega _{d}(R+r)\cos\theta \hat{i}-\omega_{d}(R+r)\sin\theta \hat{j}=\dot{x}_{A}\hat{i}+\omega_{BD}\cdot x_{A}\hat{j}$$
>  $$\begin{matrix}
\hat{j}:\omega_{BD}=-4.132\text{rad/s} \\
\hat{i}:\dot{x}_{A}=6.504\text{m/s}
\end{matrix}$$
$$\vec{a}_{P}=\cancel{ \vec{a}_{A} }+\vec{\alpha}_{d}\times \vec{r}_{p/A}-\omega_{d}^2\vec{r}_{p/A}=-\omega_{d}^2r\hat{J}\text{ where }\hat{J}=\sin\theta \hat{i}+\cos\theta \hat{j}$$
> $$=-\omega_{d}^2r\sin\theta \hat{i}-\omega_{d}^2r\cos\theta \hat{j}=\ddot{x}_{A}\hat{i}+\alpha_{BD}x_{A}\hat{i}+2\omega_{BD}\dot{x}_{A}\hat{j}-\omega_{BD}^2x_{A}\hat{i}$$
> $$\hat{i}:-\omega_{d}^2r\sin\theta=\ddot{x}_{A}-\omega_{BD}^2x_{a}=-8.138m/s$$

## "How to" with Moving Reference Frame Kinematics Equations [2D]
1. Choose your moving reference frame (observer) - recommended that you draw a stick figure of the observer on this frame
2. Draw choice of $xyz$ axes for the moving reference frame. 
3. Determine angular velocity $\vec{\omega}$ of the moving reference frame
4. Determine angular acceleration $\vec{\alpha}$ of the moving reference frame
5. Imagine yourself as the observer on the moving reference frame and answer the question "how do I see point B move if I am the observer?". Based on the answer, write down $(\vec{v}_{B/A})_{rel}$ and $(\vec{a}_{B/A})_{rel}$

# Angular Velocity and Acceleration for 3D Rotating Reference Frame Kinematics 
**For 2D problems**, the moving reference frame is rotating about a *fixed* axis that is perpendicular to the plane of the motion; specifically, this rotation is about the fixed axis. Suppose that the angular velocity of them moving reference frame is given by  $\vec{\omega}=\Omega \hat{K}$. The angular acceleration of the moving reference frame is therefore given by:
$$\vec{\alpha}=\frac{d\vec{\omega}}{dt}=\frac{d}{dt}(\Omega \hat{K})=\frac{d\Omega}{dt}\hat{K}+\Omega \frac{d\hat{K}}{dt}=\dot{\Omega}\hat{K}$$
since $\hat{K}$ is a *fixed* axis

**For 3D problems**, the differentiation to find $\vec{\alpha}$ is not so simply. $\vec{\omega}$ typically has rotation components about both fixed and moving axes. Consider the 3D system shown [[ME 27400/Dynamics, a Lecturebook.pdf#page=162|here]] where the U-shaped frame is rotating about the fixed $\hat{J}$ axis at a rate of $\omega_{1}$, and with the disk rotating about the $\hat{i}$ axis at a rate of $\omega_{2}$. This gives the total angular velocity of the disk of 
$$\vec{\omega}=\omega_{1}\hat{J}+\omega_{2}\hat{i}$$
Using the product rule of differentiation:
$$\vec{\alpha}=\frac{d\vec{w}}{dt}=\frac{d}{dt}(\omega_{1}\hat{J})+\frac{d}{dt}(\omega_{2}\hat{i})=\frac{d\omega_{1}}{dt}\hat{J}+\omega_{1} \frac{d\hat{J}}{dt}+\frac{d\omega_{2}}{dt}\hat{i}+\omega_{2} \frac{d\hat{i}}{dt}$$
Recall that $\hat{J}$ is a fixed axis $\therefore \frac{d\hat{J}}{dt}=0$. Recall also that since $\hat{i}$ is on the moving reference frame, we have $\frac{d\hat{i}}{dt}=\vec{\omega}\times \hat{i}$. Together these give:
$$\vec{\alpha}=\dot{\omega}_{1}\hat{J}+\dot{\omega}_{2}\hat{i}+\omega_{2}(\vec{\omega}\times \hat{i})=\dot{\omega}_{1}\hat{J}+\dot{\omega}_{2}\hat{i}+\omega_{2}[(\omega_{1}\hat{J}+\omega_{2}\hat{i})\times \hat{i}]=\dot{\omega}_{1}\hat{J}+\dot{\omega}_{2}\hat{i}+\omega_{2}\omega_{1}(\hat{J}\times \hat{i})$$
For the position shown in the figure, we have $\hat{J}=\hat{j}$. Therefore, the above becomes:
$$\vec{\alpha}=\dot{\omega}_{1}\hat{J}+\dot{\omega}_{2}\hat{i}-\omega_{2}\omega_{1}\hat{k}$$
>[!question] Recall that for 2D problems, when the angular speed of the observer is constant, then the angular acceleration of the observer is zero. Is this also true in 3D?
>We can write the angular acceleration of the disk for $\omega_{1}$ and $\omega_{2}$ are constant as 
> $$\vec{\alpha}=-\omega_{2}\omega_{1}\hat{k}\neq0$$
> From this we can see that, although the magnitude of the angular acceleration of the angular velocity vector is constant ($|\vec{\omega}|=\sqrt{ \omega_{1}^2+\omega_{2}^2 }=C$), the time derivative of the angular velocity vector is not zero. Observe that the orientation of the $\vec{\omega}$ vector is not fixed - at the instant shown it is moving into the plane of the page, the $-\hat{k}$ direction. This term arose from $\frac{d\hat{i}}{dt}=\vec{\omega}\times \hat{i}$. Since the direction of $\vec{\omega}$ is not constant, the time derivative $\vec{\alpha}\neq0$

 To find angular velocity and acceleration of an observer, first sum all the angular velocities in the system using $\vec{\omega}_{xyz}=\dots$ using the axes declared for the observer, then differentiate w.r.t time in order to find $\vec{\alpha}_{xyz}$
# Rotating Reference Frame Kinematics [3D]
Consider 3D motion of a rigid body with an angular velocity $\vec{\omega}$ and angular acceleration $\vec{\alpha}$ known. An observer (along with a set of $xyz$ axes) is attached to the moving rigid body. Since the observer moves along w/ the rigid body, it does not see any point on the body move $\therefore(\vec{v}_{B/A})_{rel}=(\vec{a}_{B/A})_{rel}=0,$ so
$$\vec{v}_{B}=\vec{v}_{A}+(\vec{v}_{B/A})_{rel}+\vec{\omega}\times \vec{r}_{B/A}=\vec{v}_{A}+\vec{\omega}\times \vec{r}_{B/A}$$
$$\vec{a}_{B}=\vec{a}_{A}+(\vec{a}_{B/A})_{rel}+\vec{\alpha}\times \vec{r}_{B/A}+2\vec{\omega}\times(\vec{v}_{B/A})_{rel}+\vec{\omega}\times[\vec{\omega}\times \vec{r}_{B/A}]=\vec{a}_{A}+\vec{\alpha}\times \vec{r}_{B/A}+\vec{\omega}\times[\vec{\omega}\times \vec{r}_{B/A}]$$

>[!example] The rotation rates $\omega_{1}$ and $\omega_{2}$ are constant. Determine *(a)* velocity of point $P$ at the instant when $P$ is directly above the center $A$ of the disk; *(b)* acceleration of point $P$ at the same instant. See [[ME 27400/Dynamics, a Lecturebook.pdf#page=172|figure]]
> $$\hat{J}=\hat{j},\hat{K}=\hat{k},\hat{I}=\hat{i}\text{ at instant}$$
> $$\vec{\omega}_{d}=\omega_{1}\hat{J}+\omega_{2}\hat{k}$$
> $$\vec{\alpha}_{d}=\frac{d}{dt}(\vec{\omega}_{d})=\cancel{ \dot{\omega}_{1}\hat{J} }+\cancel{ \omega_{1}\dot{\hat{J}} }+\cancel{ \dot{\omega}_{2}\hat{k} }+\omega_{2} \dot{\hat{k}}$$
> $$=\omega_{2}(\vec{\omega}_{d}\times \hat{k})=\omega_{2}(\omega_{1}\hat{j}+\omega_{2}\hat{k})\times \hat{k}=\omega_{2}\omega_{1}\hat{i}$$
> $$\vec{v}_{P}=\vec{v}_{A}+\cancel{ (\vec{v}_{P/A})_{rel} }+\vec{\omega}_{d}\times \vec{r}_{P/A}$$
> $$\vec{v}_{A}=\cancel{ \vec{v}_{O} }+\vec{\omega}_{1}\times \vec{r}_{A/O}=\omega_{1}\hat{J}\times(L\hat{i})=-\omega_{1}L\hat{k}$$
> $$\vec{v}_{P}=-\omega_{1}L\hat{k}+(\omega_{1}\hat{J}+\omega_{2}\hat{k})\times(R\hat{j})=\textcolor{green}{-\omega_{1}L\hat{k}-\omega_{2}R\hat{i}}$$
> $$\vec{a}_{P}=\vec{a}_{A}+\cancel{ (\vec{a}_{P/A})_{rel} }+\vec{\alpha}_{d}\times \vec{r}_{P/A}+2\vec{\omega}_{d}\times\cancel{ (\vec{v}_{P/A})_{rel} }+\vec{\omega}_{d}\times(\vec{\omega}_{d}\times \vec{r}_{P/A})$$
> $$\vec{a}_{A}=\cancel{ \vec{a}_{O} }+\cancel{ \vec{\alpha}_{1} }\times \vec{r}_{A/O}+\vec{\omega}_{1}\times(\vec{\omega}_{1}\times \vec{r}_{A/O})=\omega_{1}\hat{J}\times(-\omega_{1}L\hat{k})=-\omega_{1}^2L\hat{I}$$
> $$\vec{a}_{P}=-\omega_{1}^2L\hat{i}+(\omega_{2}\cdot\omega_{1}\hat{i})\times(R\hat{j})+(\omega_{1}\hat{j}+\omega_{2}\hat{k})\times(-\omega_{2}R\hat{i})$$
> $$\textcolor{green}{\vec{a}_{P}=-\omega_{1}^2L\hat{i}-\omega_{2}^2R\hat{j}+2\omega_{2}\omega_{1}R\hat{k}}$$
 