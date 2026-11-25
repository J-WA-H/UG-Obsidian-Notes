Macrostates - Specification of the system based on macroscopic properties (the actual outcome)
Examples include:
- $N$ - number of particles
- $V$ - volume
- $U$, $E$ - Internal energy
- $T$ - temperature
- $P$ - pressure

A system with constant $N$, $V$, $U$, is called a **Microcanonical ensemble**.
A system with constant $N$, $T$, $V$, is called a **Canonical ensemble**.
A system with constant chemical potential - $\mu$, $T$, $V$, is called a **Grand Canonical ensemble**.

Chemical potential is interchangeable with Fermi energy - the energy required to add or remove a particle from a system.

Microstates - A complete specification of a system (all possible outcomes).

#### Assigning Probabilities Experimentally
We can either perform an experiment an infinite amount of times and count the outcomes or have an infinite number of experiments and perform each once.
If these two methods produce the same outcome (which is almost always), it is called **ergodic**.

Example:
Lets take 4 distinguishable particles in non-degenerate energy levels of energy $0, \varepsilon,2\varepsilon, 3\varepsilon, 4\varepsilon$ such that the internal energy is $U=4\varepsilon$. What is the likely distribution of particles in these states?

| Distribution             | $n_0$           | $n_1$           | $n_2$           | $n_3$           | $n_4$          | Number of Microstates ($\Omega$) |
| ------------------------ | --------------- | --------------- | --------------- | --------------- | -------------- | -------------------------------- |
| $D_1$                    | 3               | 0               | 0               | 0               | 1              | $\frac{4!}{3!0!0!0!1!}=4$        |
| $D_2$                    | 2               | 1               | 0               | 1               | 0              | $\frac{4!}{2!1!0!1!0!}=12$       |
| $D_3$                    | 1               | 2               | 1               | 0               | 0              | $\frac{4!}{1!2!1!0!0!}=12$       |
| $D_4$                    | 2               | 0               | 2               | 0               | 0              | $\frac{4!}{2!0!2!0!0!}=6$        |
| $D_5$                    | 0               | 4               | 0               | 0               | 0              | 1                                |
| Average num of particles | $\frac{60}{35}$ | $\frac{40}{35}$ | $\frac{24}{35}$ | $\frac{12}{35}$ | $\frac{4}{35}$ | $\Omega=35$                      |
| Probability of state     | 0.43            | 0.29            | 0.17            | 0.09            | 0.03           |                                  |
These probabilities show an exponential decay of the probability as you increase energy level, consistent with the Boltzmann distribution, $A\exp\left( -\frac{\varepsilon}{k_{B}T} \right)$. This implies that from this example, which seemingly doesn't depend on temperature, we can infer the temperature of this system.

**We can obtain temperature from counting microstates**

Notation: In statistical physics we use the term "state" which is used to mean "single particle state". This state has an energy, so single particle state $i$ has energy $\varepsilon_{i}$. "Single" does not refer to number of particles but the **single energy $\varepsilon_{i}$** of a state. We can put the number of particles $n_i$ in state $\varepsilon_{i}$.
Then $N=\sum_{i}n_{i}$ and $U=\sum_{i}n_{i}\varepsilon_{i}$.