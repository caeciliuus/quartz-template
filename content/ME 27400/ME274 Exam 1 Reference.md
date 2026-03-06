---
publish: true
created: 2026-02-11T12:06:52.946-05:00
modified: 2026-02-11T21:51:03.109-05:00
tags:
  - S2
  - studyguide
  - exam
  - me274
cssclasses: ""
---

# Particle Kinematics
- Path description given by $\textcolor{green}{\vec{a}=\dot{v}\hat{e}_{t}+\frac{v^2}{\rho}\hat{e}_{n}}$
- When given a position function e.g $y(x)$ and one component of velocity e.g $v_{y}(t)$, use chain rule to find the other component of velocity like $\frac{dy}{dt}=\frac{dy}{dx} \frac{dx}{dt}\to v_{x}=\frac{v_{y}}{y'(x)}$
- *Rate of change of speed* is not the same as the magnitude of the acceleration, but rather $\frac{dv}{dt}=\vec{a}\cdot \hat{t}=\frac{\vec{v}\cdot \vec{a}}{|\vec{v}|}$
	- $\dot{v}$ is equivalent to tangential acceleration
- Radius of curvature $\rho=\frac{(1+(y')^2)^{3/2}}{|y''|}$ 
	- If asked for $\rho$ and you've already found $\vec{v},\vec{a},\dot{v}$ (where $\dot{v}=a_{t}$), radius of curvature can also be found using the formula $|\vec{a}|=\sqrt{ a_{t}^2+a_{n}^2 }=\sqrt{ \dot{v}^2+\left( \frac{|\vec{v}|^2}{\rho} \right)^2 }\to \rho=\frac{|\vec{v}|^2}{\sqrt{ |\vec{a}|^2-\dot{v}^2 }}$
- $a_{n}=\frac{v^2}{\rho}=\vec{a}\cdot \hat{e}_{n}$
- $\dot{v}_{P}=a_{t}=\vec{a}\cdot \hat{e}_{t}$
# Rigid Body Kinematics
- When given questions with mlutiple links / pulleys over a single length of cable: **(1)** determine which lengths aren't changing (based on constraints); **(2)** sum the lengths of the cable; **(3)** differentiate w.r.t time

> [!example] An inextensible cable connects block A to ground at E, with the cable being wrapped around two fixed pulleys at B and C, and a moveable pulley at D. When pulley D is at the location $(x_{D},y_{D})=(0.3,0.4)m,$ the center of pulley D is known to have a velocity of $\vec{v}_{D}=(2\hat{i})m/s$. Determine the speed of block A at that instant. Use $h=0.8m$. Assume pulleys to have small radii.
> ![[Attachments/Pasted image 20260211153034.png|right|200]]
> $$L=r_{ED}+r_{DC}+r_{CB}+s_{A}$$
$$\frac{d}{dt} (L)=\dot{r}_{ED}+\dot{r}_{DC}+\dot{s}_{A}=0$$
$$r_{ED}=(x_{D}^2+(h-y_{D})^2)^{-1/2},r_{DC}=(x_{D}^2+y_{D}^2)^{1/2}$$
$$\dot{r}_{ED}=\frac{1}{2}(x_{D}^2+(h-y_{D})^2)^{-1/2}\cdot2x_{D}\dot{x}_{D}+\cancel{ 2(h-y_{D})\dot{y}_{D} }=\frac{x_{D}\dot{x}_{D}}{r_{ED}}$$
$$\dot{r}_{DC}=\frac{1}{2}(x_{D}^2+y_{D}^2)^{-1/2}\cdot2x_{D}\dot{x}_{D}+\cancel{ 2y_{D}\dot{y}_{D} }=\frac{x_{D}\dot{x}_{D}}{r_{DC}}$$
$$r_{ED}=0.5=r_{DC},\dot{r}_{DC}=1.2m/s=\dot{r}_{ED}\to \dot{s}_{A}=-1.2-1.2=-2.4m/s,\boxed{|v_{A}|=2.4m/s}$$

- For instantaneous center problems, velocity of points linked to points constrained to zero motion is perpendicular to the link itself. Draw all of those first before going to find $IC$
- Points closer to their $IC$ will have a higher $\omega\to v=|\omega|IC$ 

$$\hat{i}\times \hat{j}=\hat{k}$$
$$\hat{j}\times \hat{k}=\hat{i}$$
$$\hat{k}\times \hat{i}=\hat{j}$$