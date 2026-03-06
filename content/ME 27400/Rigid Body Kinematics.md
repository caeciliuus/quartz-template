---
publish: true
created: 2026-02-02T14:58:09.868-05:00
modified: 2026-02-02T16:24:03.447-05:00
tags:
  - S2
  - me274
  - lecture
cssclasses: ""
---

The equations below relate the kinematics of any two points A & B on the same rigid body while the body executes planar motion ($\vec{r}_{B/A}$ is the vector from point $A$ to $B$)
$$\vec{v}_{B}=\vec{v}_{A}+\vec{\omega}\times\vec{r}_{B/A}$$
$$\vec{a}_{B}=\vec{a}_{A}+\vec{\alpha} \times \vec{r}_{B/A}+\vec{\omega}\times[\vec{\omega}\times \vec{r}_{B/A}]$$
- The vectors $\vec{\omega}=\omega \hat{k}$ and $\vec{\alpha}=\alpha \vec{k}$ are the angular velocity and angular acceleration of the rigid body  respectively. These are properties of the motion of the rigid body and are the same regardless of which points $A$ and $B$ are used in the above equation. That is, a rigid body has one (and only one) angular velocity, and only one angular accelreation
- The direction $\hat{k}$ for the angular velocity and acceleration vectors denote the axis about which the body rotates. The signs of $\omega$ and $\alpha$ provide the sense of rotational velocity and acceleration. Suppose that $\hat{k}$ points out of the page. Then, by the right hand rule, a positive sign denoties counterclockwise motion, and a negative sign denotes clockwise rotation

If $A$ and $B$ both line in a plane perpendicular to the $\hat{k}$ direction then the last term on the right hand side of the acceleration equation simplifies to:
$$\vec{\omega}\times(\vec{\omega}\times \vec{r}_{{B/A}})=(\omega \hat{k})\times[(\omega \hat{k})\times(x \hat{i}+y\hat{j})]$$
$$=(\omega \hat{k})\times(x\omega \hat{j}-y\omega \hat{i})=-x\omega^2\hat{i}-y\omega^2\hat{j}$$
$$=-\omega^2(x \hat{i}+y\hat{j})=-\omega^2 \vec{r}_{B/A}$$
In this case, the form of the acceleration simplifies to $\mathbf{\vec{a}_{B}=\vec{a}_{A}+\vec{\alpha}\times \vec{r}_{{B/A}}}-\omega^2\vec{r}_{B/A}$

The relative velocity vector $\vec{v}_{B/A}=\vec{v}_{B}-\vec{v}_{A}=\vec{\omega}\times \vec{r}_{B/A}$ is always perpendicular to the line connecting points $A$ and $B$. However, the relative accerleation vector $\vec{a}_{B/A}=\vec{a}_{B}-\vec{a}_{A}=\vec{\alpha}\times \vec{r}_{B/A}-\omega^2\vec{r}_{B/A}$ is *not* perpendicular to the line connecting points $A$ and $B$

---

- Rolling without slipping: at contact point, there's neither velocity nor acceleration in the $x$-direction
- Force of friction $f_{s}$ keeps the wheel from slipping 
- No acceleration/velocity in the x-direction during rolling w/o slipping, but there is still an acceleration force in the $y$-direction to oppose the normal force required for friction to exist