# Cartesian, Polar Coordinates, and Basis Vectors: Example Problems and Solutions

## Coordinate Transformations

### Problem 1
Convert the following points from Cartesian coordinates $(x, y)$ to polar coordinates $(r, \theta)$:

a) $(1, 1)$

b) $(-3, 4)$

c) $(0, -2)$

### Solution 1

a) $(1, 1)$
$$r = \sqrt{1^2 + 1^2} = \sqrt{2}$$
$$\theta = \arctan\left(\frac{1}{1}\right) = \frac{\pi}{4}$$
$$\left(\sqrt{2}, \frac{\pi}{4}\right)$$

b) $(-3, 4)$
$$r = \sqrt{(-3)^2 + 4^2} = \sqrt{9 + 16} = 5$$
$$\theta = \arctan\left(\frac{4}{-3}\right) + \pi = \pi - \arctan\left(\frac{4}{3}\right)$$
$$\left(5, \pi - \arctan\left(\frac{4}{3}\right)\right)$$

c) $(0, -2)$
$$r = \sqrt{0^2 + (-2)^2} = 2$$
$$\theta = \frac{3\pi}{2}$$
$$\left(2, \frac{3\pi}{2}\right)$$

### Problem 2
Convert the following points from polar coordinates $(r, \theta)$ to Cartesian coordinates $(x, y)$:

a) $(2, \pi/4)$

b) $(5, -\pi/6)$

c) $(1, 3\pi/2)$

### Solution 2

a) $(2, \pi/4)$
$$x = 2 \cos\left(\frac{\pi}{4}\right) = 2 \cdot \frac{\sqrt{2}}{2} = \sqrt{2}$$
$$y = 2 \sin\left(\frac{\pi}{4}\right) = 2 \cdot \frac{\sqrt{2}}{2} = \sqrt{2}$$
$$(\sqrt{2}, \sqrt{2})$$

b) $(5, -\pi/6)$
$$x = 5 \cos\left(-\frac{\pi}{6}\right) = 5 \cdot \frac{\sqrt{3}}{2} = \frac{5\sqrt{3}}{2}$$
$$y = 5 \sin\left(-\frac{\pi}{6}\right) = 5 \cdot \left(-\frac{1}{2}\right) = -\frac{5}{2}$$
$$\left(\frac{5\sqrt{3}}{2}, -\frac{5}{2}\right)$$

c) $(1, 3\pi/2)$
$$x = 1 \cos\left(\frac{3\pi}{2}\right) = 1 \cdot 0 = 0$$
$$y = 1 \sin\left(\frac{3\pi}{2}\right) = 1 \cdot (-1) = -1$$
$$(0, -1)$$

## Basis Vectors

### Problem 1
Express the Cartesian basis vectors $(\mathbf{e}_x, \mathbf{e}_y)$ in terms of the polar basis vectors $(\mathbf{e}_r, \mathbf{e}_\theta)$.

### Solution 1
$$\mathbf{e}_x = \cos(\theta) \mathbf{e}_r - \sin(\theta) \mathbf{e}_\theta$$
$$\mathbf{e}_y = \sin(\theta) \mathbf{e}_r + \cos(\theta) \mathbf{e}_\theta$$

### Problem 2
Express the polar basis vectors $(\mathbf{e}_r, \mathbf{e}_\theta)$ in terms of the Cartesian basis vectors $(\mathbf{e}_x, \mathbf{e}_y)$.

### Solution 2
$$\mathbf{e}_r = \cos(\theta) \mathbf{e}_x + \sin(\theta) \mathbf{e}_y$$
$$\mathbf{e}_\theta = -\sin(\theta) \mathbf{e}_x + \cos(\theta) \mathbf{e}_y$$

### Problem 3
Given a vector $\mathbf{v} = 3\mathbf{e}_x + 4\mathbf{e}_y$, express $\mathbf{v}$ in terms of the polar basis vectors $(\mathbf{e}_r, \mathbf{e}_\theta)$ at the point $(1, 1)$.

### Solution 3
At the point $(1, 1)$, we have $r = \sqrt{2}$ and $\theta = \pi/4$.

The radial component is:
$$v_r = \mathbf{v} \cdot \mathbf{e}_r = (3\mathbf{e}_x + 4\mathbf{e}_y) \cdot (\cos(\theta)\mathbf{e}_x + \sin(\theta)\mathbf{e}_y) = 3\cos(\theta) + 4\sin(\theta)$$

At $\theta = \pi/4$:
$$v_r = 3 \cdot \frac{\sqrt{2}}{2} + 4 \cdot \frac{\sqrt{2}}{2} = \frac{7\sqrt{2}}{2}$$

The angular component is:
$$v_\theta = \mathbf{v} \cdot \mathbf{e}_\theta = (3\mathbf{e}_x + 4\mathbf{e}_y) \cdot (-\sin(\theta)\mathbf{e}_x + \cos(\theta)\mathbf{e}_y) = -3\sin(\theta) + 4\cos(\theta)$$

At $\theta = \pi/4$:
$$v_\theta = -3 \cdot \frac{\sqrt{2}}{2} + 4 \cdot \frac{\sqrt{2}}{2} = \frac{\sqrt{2}}{2}$$

Therefore:
$$\mathbf{v} = \frac{7\sqrt{2}}{2} \mathbf{e}_r + \frac{\sqrt{2}}{2} \mathbf{e}_\theta$$

## Vector Transformations

### Problem 1
A vector $\mathbf{v}$ has components $(2, 3)$ in the Cartesian basis. What are its components in the polar basis at the point $(1, \pi/4)$?

### Solution 1
The transformation from Cartesian to polar components is given by:
$$\begin{pmatrix} v_r \\ v_\theta \end{pmatrix} = \begin{pmatrix} \cos(\theta) & \sin(\theta) \\ -\sin(\theta) & \cos(\theta) \end{pmatrix} \begin{pmatrix} v_x \\ v_y \end{pmatrix}$$

At $\theta = \pi/4$:
$$v_r = 2\cos\left(\frac{\pi}{4}\right) + 3\sin\left(\frac{\pi}{4}\right) = 2 \cdot \frac{\sqrt{2}}{2} + 3 \cdot \frac{\sqrt{2}}{2} = \frac{5\sqrt{2}}{2}$$

$$v_\theta = -2\sin\left(\frac{\pi}{4}\right) + 3\cos\left(\frac{\pi}{4}\right) = -2 \cdot \frac{\sqrt{2}}{2} + 3 \cdot \frac{\sqrt{2}}{2} = \frac{\sqrt{2}}{2}$$

The components are $\left(\frac{5\sqrt{2}}{2}, \frac{\sqrt{2}}{2}\right)$.

### Problem 2
A vector field is given by $\mathbf{F} = r^2 \mathbf{e}_r$. Express this vector field in Cartesian coordinates.

### Solution 2
$$\mathbf{F} = r^2 (\cos(\theta) \mathbf{e}_x + \sin(\theta) \mathbf{e}_y)$$

$$\mathbf{F} = (r^2 \cos(\theta)) \mathbf{e}_x + (r^2 \sin(\theta)) \mathbf{e}_y$$

Since $x = r\cos(\theta)$ and $y = r\sin(\theta)$, we have $r^2 = x^2 + y^2$ and $r = \sqrt{x^2 + y^2}$.

Therefore:
$$\mathbf{F} = (r \cdot x) \mathbf{e}_x + (r \cdot y) \mathbf{e}_y = \sqrt{x^2 + y^2} (x \mathbf{e}_x + y \mathbf{e}_y)$$