---
publish: true
created: 2026-01-20T16:32:55.927-05:00
modified: 2026-02-11T10:54:52.755-05:00
tags:
  - S2
  - me274
  - lecture
cssclasses: ""
---

# I. Cartesian Description
- Given position function $f(x,y)=c$, apply implicit differentiation with respect to time to find $v(t)$ then differentiate again for $a(t)$
- Remember chain rule when finding $v(t),a(t)\to \vec{v}=\frac{d\vec{r}}{dt} \frac{ds}{dt}=v \frac{d\vec{r}}{ds}$ where $\frac{d\vec{r}}{ds}$ is the speed of the particle

>[!note] 
>$\dot{x}$ denotes first derivative of $x$ w.r.t time while $\ddot{x}$ denotes second derivative of $x$ w.r.t time




**Q1:** How would the results change if the slot moved downward instead of upward?  
**Q2:** Can the same method be generalised for a circular ring constraint?  
**Q3:** How would introducing a time-varying slot speed \(v(t)\) affect the acceleration analysis?

# II. Path Description 
- ![[Attachments/Pasted image 20260120164355.png|right|167]]Sometimes its easier to describe position as a function of distance, i.e. $x(s)$, called **path description** 
- $\frac{d\vec{r}}{ds}=\hat{e}_{t}$ (or $\hat{u}_{t}$ in image to the right) unit vector tangent to the path of P, therefore $\vec{v}=v\hat{e}_{t}$
$$\vec{a}=\frac{d\vec{v}}{dt}=\frac{dv}{dt}\hat{e}_{t}+v \frac{d\hat{e}_{t}}{dt}=\dot{v}\hat{e}_{t}+v \frac{d\hat{e}_{t}}{ds} \frac{ds}{dt}\to \textcolor{green}{\vec{a}=\dot{v}\hat{e}_{t}+v^2 \frac{d\hat{e}_{t}}{d\theta} \frac{d\theta}{ds}}$$
- Letting $\theta$ be the angle between $\hat{i}$ and $\hat{e}_{t}$, $C$ be the "center of curvature" (center of circle tangent to the path having the same curvature of the path), and $\rho$ be the "radius of curvature" of the path, we get $\frac{d\hat{e}_{t}}{d\theta} \frac{d\theta}{ds} =\frac{\hat{e}_{n}}{\rho}$ so $\textcolor{green}{\vec{a}=\dot{v}\hat{e}_{t}+\frac{v^2}{\rho}\hat{e}_{n}}$
	- For a general path in terms of its cartesian coordinates $y=y(x)$, radius of curvature can be calculated from $\rho=\frac{\left[ 1+\left( \frac{dy}{dx} \right)^2 \right]^{3/2}}{\left| \frac{d^2y}{dx^2} \right|}$
- We see acceleration has two components: that which is *normal* to the path, $\frac{v^2}{\rho}\hat{e}_{n}$, which is always directed inward to the path, and that which is *tangent* to the path, $\dot{v} \hat{e}_{t}$
	- Magnitude of acceleration is given by the square root of the sum of the squares of its path components: $|\vec{a}|=\sqrt{ \dot{v}^2+\left( \frac{v^2}{\rho} \right)^2 }$
	- Do not confuse "rate of change of speed" with magnitude of acceleration -> $\dot{v}\neq|\vec{a}|$
# III. Polar Description ![[Attachments/Pasted image 20260120171109.png|right|162]]
- For polar description, two unit vectors will be used: $\hat{e}_r$ pointing from $O$ to point $P$, and $\hat{e}_{\theta}$ perpendicular to $\hat{e}_{r}$, pointing in the "positive $\theta$ direction"
- Position vector of $P$ written as $\vec{r}=r\hat{e}_r$, velocity $\vec{v}=\frac{d}{dt}(r\hat{e}_r)=\frac{dr}{dt}\hat{e}_{r}+r d\hat{e}_{r}\to \textcolor{green}{\vec{v}=\dot{r}\hat{e}_{r}+r\theta \hat{e}_{\theta}}$
	- $\dot{r} \hat{e}_{r}$ represents change in magnitude of $r$ and $r\theta \hat{e}_{\theta}$ represents change in direction of $r$

$$
\vec{a}
= \frac{d}{dt}\!\left(\dot{r}\,\hat{e}_r\right)
+ \frac{d}{dt}\!\left(r\dot{\theta}\,\hat{e}_\theta\right)
= \ddot{r}\,\hat{e}_r
+ \dot{r}\,\frac{d\hat{e}_r}{dt}
+ r\ddot{\theta}\,\hat{e}_\theta
+ \dot{r}\dot{\theta}\,\hat{e}_\theta
+ r\dot{\theta}\,\frac{d\hat{e}_\theta}{dt} 
$$
$$\to\textcolor{green}{\vec{a}=(\ddot{r}-r\dot{\theta}^2)\hat{e}_{r}+(r \ddot{\theta}+2\dot{r}\dot{\theta})\hat{e}_{\theta}}$$
- Values for the components of these vectors depend on your choice of the point $O$ so carefully define it @ beginning of problem if not already given (usually is)
- When path of $P$ is given as $r=r(\theta)$, you will need to use *chain rule of differentiation* to find the time derivatives $\dot{r}=\frac{dr}{dt}$ and $\ddot{r}=\frac{d^2r}{dt^2}$
# IV. Summary & Converting To/From Coordinate Systems
## 1. Always start w/ geometry
- Cartesian: $\vec{r}=x \hat{i}+y \hat{j}$
- Polar: $r=r \hat{e}_{r}$ with $x=r\cos\theta$ and $y=r\sin\theta$
- Path: position is implicit - motion described along a curve using arc length $s$
### 1a. Express unit vectors correctly, specifically *polar*
- $\hat{e}_{r}=\cos\theta \hat{i}+\sin\theta \hat{j}$
- $\hat{e}_{\theta}=-\sin\theta \hat{i}+\cos\theta \hat{j}$
- Time derivatives $\dot{\hat{e}}_{r}=\hat{\theta} \hat{e}_{\theta}$, $\dot{\hat{e}}_{\theta}=-\dot{\theta}\hat{e}_{r}$
## 2. Differentiate position -> velocity
- Cartesian: $\vec{v}=\dot{x} \hat{i}+\dot{y} \hat{j}$
- Polar: $\vec{v}=\dot{r} \hat{e}_{r}+r\dot{\theta}\hat{e}_{\theta}$
- Interpretation: $\dot{r}$ is radial speed while $r\dot{\theta}$ is transverse [angular] speed
## 3. Differentiate velocity -> acceleration
- Cartesian: $\vec{a}=\ddot{x} \hat{i}+\ddot{y}\hat{j}$
- Polar: $\vec{a}=(\ddot{r}-r\dot{\theta}^2)\hat{e}_{r}+(r \ddot{\theta}+2\dot{r} \dot{\theta})\hat{e}_{\theta}$
- Key terms
	- $-r \dot{\theta}^2$ is centripetal
	- $2\dot{r} \dot{\theta}$ is "Coriolis-type coupling"
## 4. Path ($t-n$ coordinates)
- Used when trajectory is known but not easily expressed in $x-y$
- Velocity: $\vec{v}=v \hat{t}$
- Acceleration: $\vec{a}=\dot{v} \hat{t}+ \frac{v^2}{\rho} \hat{n}$
	- $\rho$ is radius of curvature & $\hat{n}$ is point toward centre of curvature
## 5. Converting between systems
### 5a. Polar -> cartesian
1. Write vectors in $\hat{e}_{r},\hat{e}_{\theta}$
2. Substitute unit vectors using trig
3. Collect $\hat{i},\hat{j}$
### 5b. Cartesian -> polar
1. Compute $r,\theta$
2. Project vectors: $v_{r}=v \cdot \hat{e}_{r},v_{\theta}=v\cdot \hat{e}_{\theta}$
### 5c. Polar -> path
- At any instant:
	- $\hat{t}$ aligns w/ velocity direction
	- $\hat{n}$ points toward instanteanous center of curvature
- Use geometry to relate $r,\theta$ to curvature $\rho$
## Other
### How to choose the coordinate system
- Straight or piecewise straight motion -> cartesian
- Rotation about a point -> polar
- Motion along a known curve -> path
### Common failure modes to avoid
- Treating polar unit vectors as constant
- Forgetting $2\dot{r}\dot{\theta}$
- Mixing $\theta$ (geometry) with $\dot{\theta}$ (kinematics)
- Using t-n without checking curvature direction