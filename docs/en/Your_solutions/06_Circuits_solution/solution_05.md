

## 5 Kirchhoff's Laws

To find the currents $I_1$, $I_2$, and $I_3$ going through the resistors $R_1$, $R_2$, and $R_3$ (where $R_3$ represents the internal resistance $r_w = 1\ \Omega$ of the right loop), we apply Kirchhoff's laws.

### 1. Define Current Directions and Loops

* Let $I_1$ be the current in the left loop, flowing counter-clockwise (out of the positive terminal of $\mathcal{E}_1$).
* Let $I_3$ be the current in the right loop, flowing counter-clockwise (out of the positive terminal of $\mathcal{E}_2$).
* Let $I_2$ be the current flowing downward through the shared central resistor $R_2$.

---

### 2. Kirchhoff's Current Law (KCL)

At the top-right node where the branches meet:


$$I_1 + I_3 = I_2$$

---

### 3. Kirchhoff's Voltage Law (KVL)

**Left Loop (Counter-clockwise):**


$$\mathcal{E}_1 - I_1 R_1 - I_2 R_2 - I_1 r_w = 0$$

$$4.5 - 20I_1 - 10I_2 - 1I_1 = 0$$

$$21I_1 + 10I_2 = 4.5 \quad \text{--- (Equation 1)}$$

**Right Loop (Counter-clockwise):**


$$\mathcal{E}_2 - I_3 r_w - I_2 R_2 = 0$$

$$9 - 1I_3 - 10I_2 = 0$$

$$1I_3 + 10I_2 = 9 \quad \text{--- (Equation 2)}$$

---

### 4. Solve the System of Equations

Substitute $I_3 = I_2 - I_1$ into Equation 2:


$$(I_2 - I_1) + 10I_2 = 9$$

$$-I_1 + 11I_2 = 9 \implies I_1 = 11I_2 - 9$$

Substitute this expression for $I_1$ into Equation 1:


$$21(11I_2 - 9) + 10I_2 = 4.5$$

$$231I_2 - 189 + 10I_2 = 4.5$$

$$241I_2 = 193.5$$

$$I_2 = \frac{193.5}{241} \approx 0.803\text{ A}$$

Now, find $I_1$:


$$I_1 = 11(0.803) - 9 \approx -0.167\text{ A}$$


*(The negative sign indicates that $I_1$ actually flows clockwise, opposite to our assumed direction).*

Now, find $I_3$:


$$I_3 = I_2 - I_1 = 0.803 - (-0.167) \approx 0.970\text{ A}$$

---

### Final Answer

* **$I_1 = -0.167\text{ A}$** (or $0.167\text{ A}$ in the clockwise direction)
* **$I_2 = 0.803\text{ A}$** (downward through $R_2$)
* **$I_3 = 0.970\text{ A}$** (counter-clockwise through the right loop)

