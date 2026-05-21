

## 5 Kirchhoff's Laws

Let the currents be:

* (I_1) through (R_1=20\Omega) (left branch),
* (I_2) through (R_2=10\Omega) (middle branch),
* (I_3) through the right branch with source (E_2).

We’ll use Kirchhoff’s laws.

---

# 1. Choose current directions

Assume:

* (I_1): clockwise in the left loop,
* (I_3): clockwise in the right loop,
* (I_2): downward through (R_2).

At the top junction, currents (I_1) and (I_3) flow into the shared resistor branch, so:

[
I_2 = I_1 + I_3
]

This is Kirchhoff’s Current Law (KCL).

---

# 2. Left loop equation

The left loop contains:

* resistor (R_1=20\Omega),
* internal resistance (r_1=1\Omega),
* shared resistor (R_2=10\Omega),
* source (E_1=4.5\text{ V}).

Applying Kirchhoff’s Voltage Law (KVL):

[
20I_1 + 1I_1 + 10I_2 = 4.5
]

So:

[
21I_1 + 10I_2 = 4.5
\tag{1}
]

---

# 3. Right loop equation

Right loop contains:

* internal resistance (r_2=1\Omega),
* resistor (R_2=10\Omega),
* source (E_2=9\text{ V}).

KVL gives:

[
1I_3 + 10I_2 = 9
]

or

[
I_3 + 10I_2 = 9
\tag{2}
]

---

# 4. Use the junction equation

[
I_2 = I_1 + I_3
\tag{3}
]

Now solve the system.

---

# 5. Solve the equations

From (2):

[
I_3 = 9 - 10I_2
]

Using (3):

[
I_2 = I_1 + 9 - 10I_2
]

[
11I_2 = I_1 + 9
]

[
I_1 = 11I_2 - 9
\tag{4}
]

Substitute into (1):

[
21(11I_2 - 9) + 10I_2 = 4.5
]

[
231I_2 - 189 + 10I_2 = 4.5
]

[
241I_2 = 193.5
]

[
I_2 \approx 0.803\text{ A}
]

Now compute the others.

From (4):

[
I_1 = 11(0.803) - 9
]

[
I_1 \approx -0.163\text{ A}
]

From (2):

[
I_3 = 9 - 10(0.803)
]

[
I_3 \approx 0.967\text{ A}
]

---

# 6. Final answer

[
\boxed{I_1 \approx -0.16\text{ A}}
]

[
\boxed{I_2 \approx 0.80\text{ A}}
]

[
\boxed{I_3 \approx 0.97\text{ A}}
]

The negative sign for (I_1) means the actual current through (R_1) flows opposite to the direction we originally assumed.

