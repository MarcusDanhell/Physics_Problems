

## 5 Kirchhoff's Laws

### Step 1: Define Nodes and Current Directions

Let's identify the key junctions (nodes) in the circuit:

* **Node X:** The top junction above the shared resistor $R_2$.
* **Node Y:** The bottom junction below $R_2$, which we will set as our reference ground ($V_Y = 0\ \text{V}$).

We assume the following standard directions for the currents entering/leaving Node X:

* $I_1$: Flows clockwise in the left loop (from left to right through $R_1$, entering Node X).
* $I_2$: Flows downwards through the center branch (from Node X to Node Y through $R_2$).
* $I_3$: Flows upwards through the right branch (entering Node X from the right loop).

---

### Step 2: Apply Kirchhoff's Current Law (KCL)

According to KCL, the sum of currents entering a node equals the sum of currents leaving it. At Node X:


$$I_1 + I_3 = I_2$$

---

### Step 3: Express Currents using Ohm's Law

Given values from the problem:

* $R_1 = 20\ \Omega$
* $R_2 = 10\ \Omega$
* Left loop internal resistance $r_w = 1\ \Omega$ (total left branch resistance is $R_1 + r_w = 21\ \Omega$)
* Right loop internal resistance $r_w = 1\ \Omega$
* Voltage sources: $\mathcal{E}_1 = 4.5\ \text{V}$ and $\mathcal{E}_2 = 9\ \text{V}$

We express each current in terms of the unknown node voltage $V_X$:

1. **Left Branch ($I_1$):** Moving from ground up through the source $\mathcal{E}_1$ gives a potential boost of $+4.5\ \text{V}$:

$$I_1 = \frac{4.5 - V_X}{21}$$


2. **Middle Branch ($I_2$):** 
$$I_2 = \frac{V_X}{10}$$


3. **Right Branch ($I_3$):** Moving from ground up through the source $\mathcal{E}_2$ gives a potential boost of $+9\ \text{V}$:

$$I_3 = \frac{9 - V_X}{1}$$



---

### Step 4: Solve for the Node Voltage $V_X$

Substitute the branch current expressions into the KCL equation:


$$\frac{4.5 - V_X}{21} + (9 - V_X) = \frac{V_X}{10}$$

To eliminate denominators, multiply the entire equation by $210$ (the least common multiple of 21 and 10):


$$10(4.5 - V_X) + 210(9 - V_X) = 21V_X$$

$$45 - 10V_X + 1890 - 210V_X = 21V_X$$

$$1935 - 220V_X = 21V_X$$

$$1935 = 241V_X$$

$$V_X = \frac{1935}{241} \approx 8.029\ \text{V}$$

---

### Step 5: Calculate the Final Currents

* **Current $I_1$:**

$$I_1 = \frac{4.5 - \frac{1935}{241}}{21} = -\frac{81}{482}\ \text{A} \approx -0.168\ \text{A}$$



*(The negative sign simply indicates that $I_1$ actually flows counter-clockwise, away from Node X).*
* **Current $I_2$:**

$$I_2 = \frac{\frac{1935}{241}}{10} = \frac{387}{482}\ \text{A} \approx 0.803\ \text{A}$$


* **Current $I_3$:**

$$I_3 = \frac{9 - \frac{1935}{241}}{1} = \frac{234}{241}\ \text{A} \approx 0.971\ \text{A}$$



---

### Summary of Results

| Current | Exact Fraction Value | Decimal Value |
| --- | --- | --- |
| **$I_1$** | $-\frac{81}{482}\ \text{A}$ | **$-0.168\ \text{A}$** |
| **$I_2$** | $\frac{387}{482}\ \text{A}$ | **$0.803\ \text{A}$** |
| **$I_3$** | $\frac{234}{241}\ \text{A}$ | **$0.971\ \text{A}$** |
