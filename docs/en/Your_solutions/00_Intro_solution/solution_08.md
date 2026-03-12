## 9. Optimization: Rectangle Under a Curve

To find the dimensions of the rectangle with the maximum area under the curve $y = 3 - x^2$ in the first quadrant, we follow these steps:

### 1. Define the Area Function

A rectangle in the first quadrant with one vertex at the origin $(0,0)$ and the opposite vertex on the curve $(x, y)$ has:

* **Width:** $x$
* **Height:** $y = 3 - x^2$

The area $A$ is the product of width and height:


$$A(x) = x(3 - x^2) = 3x - x^3$$

### 2. Find the Critical Points

To maximize the area, we take the derivative of $A(x)$ with respect to $x$ and set it to zero:


$$A'(x) = 3 - 3x^2$$

$$3 - 3x^2 = 0 \implies x^2 = 1 \implies x = 1$$


*(Note: We ignore $x = -1$ as the rectangle is in the first quadrant.)*

### 3. Verify the Maximum

Using the second derivative test:


$$A''(x) = -6x$$


At $x = 1$, $A''(1) = -6$. Since the second derivative is negative, the area is at a **maximum** at $x = 1$.

### 4. Determine Dimensions

* **Width:** $x = 1$
* **Height:** $y = 3 - (1)^2 = 2$

The dimensions for the maximum area are **1 unit wide** and **2 units high**, resulting in a maximum area of **2 square units**.

---

Would you like me to show the step-by-step derivation for the infinite series in Task 10?
