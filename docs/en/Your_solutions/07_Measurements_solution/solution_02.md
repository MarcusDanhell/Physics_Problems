## 2. Propagation of Error 2

To find the area of the rectangular plate and its associated uncertainty, we follow a two-step process: calculating the nominal area and then propagating the uncertainties of the length and width.

### 1. Nominal Area Calculation

The formula for the area ($A$) of a rectangle is:


$$A = L \times W$$

Given:

* Length, $L = 15.3 \text{ cm}$
* Width, $W = 8.4 \text{ cm}$

Substituting these values gives:


$$A = 15.3 \text{ cm} \times 8.4 \text{ cm} = 128.52 \text{ cm}^2$$

---

### 2. Uncertainty Propagation

Depending on the physics or statistics curriculum, there are two standard methods used to calculate the uncertainty in a product ($\Delta A$).

#### Method A: Quadrature (Random/Independent Errors)

If the measurements for length and width are independent, their errors are likely to partially cancel out. The fractional uncertainty of the area is found using the Pythagorean addition (quadrature) of the fractional uncertainties:

$$\frac{\Delta A}{A} = \sqrt{\left(\frac{\Delta L}{L}\right)^2 + \left(\frac{\Delta W}{W}\right)^2}$$

Given uncertainties: $\Delta L = 0.1 \text{ cm}$ and $\Delta W = 0.1 \text{ cm}$:


$$\frac{\Delta A}{128.52} = \sqrt{\left(\frac{0.1}{15.3}\right)^2 + \left(\frac{0.1}{8.4}\right)^2}$$

$$\frac{\Delta A}{128.52} = \sqrt{(0.006536)^2 + (0.011905)^2}$$

$$\frac{\Delta A}{128.52} = \sqrt{0.00004272 + 0.00014173} = \sqrt{0.00018445} \approx 0.01358$$

Now, solve for $\Delta A$:


$$\Delta A = 128.52 \times 0.01358 \approx 1.75 \text{ cm}^2$$

#### Method B: Linear / Worst-Case (Dependent Errors)

If the errors are not independent or you are looking for the absolute maximum upper bound of the error, the fractional uncertainties are added directly:

$$\frac{\Delta A}{A} = \frac{\Delta L}{L} + \frac{\Delta W}{W}$$

Multiplying both sides by $A = L \times W$ simplifies this to:


$$\Delta A = W \cdot \Delta L + L \cdot \Delta W$$

$$\Delta A = (8.4 \times 0.1) + (15.3 \times 0.1) = 0.84 + 1.53 = 2.37 \text{ cm}^2$$

---

### 3. Final Rounding and Significant Figures

Experimental uncertainties are generally rounded to **one significant figure** (or occasionally two if the leading digit is 1).

* Using **Method A (Quadrature)**, $\Delta A \approx 1.75 \text{ cm}^2 \rightarrow 2 \text{ cm}^2$.
* Using **Method B (Linear)**, $\Delta A \approx 2.37 \text{ cm}^2 \rightarrow 2 \text{ cm}^2$.

Since the uncertainty is rounded to the units place ($\pm 2$), the nominal value of the area must also be rounded to the same decimal place ($128.52 \rightarrow 129$).

### Final Answer:

$$A = (129 \pm 2) \text{ cm}^2$$
