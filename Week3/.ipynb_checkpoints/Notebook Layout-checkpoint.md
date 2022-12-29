# The Purpose of Quantum Computing

The goal of studying Quantum Computing is to observe what problems these new computers offer a <u>significant speedup</u> to when compared to their classical counterparts.



## Big $O$ and P vs. NP

In theoretical computer science, there is the concept of the **complexity classes**, P and NP.

- P (*Polynomial Time*) refers to problems that a computer algorithm can solve is a <u>non-exponential</u> amount of time.
  - This is referring to Constant time: $O(1)$ to Polynomial time: $O(n^k)$ for some positive constant $k$
- NP (*Non-deterministic Polynomial Time*) refers to problems with answers that can be <u>verified</u> in polynomial time but cannot be solved in polynomial time on a deterministic machine
  - This is referred to being solvable in polynomial time on a non-deterministic machine



### New Challenger: BQP

**Bounded-error Quantum Polynomial Time** refers to the complexity class where there exists a quantum algorithm that can solve a problem in polynomial time <u>with a high probability</u> of being correct.

- This probability must be, at minimum, $2/3$ of the total outcomes, leaving the other $1/3$ as "error/wrong outputs"
- Quantum Computers as they stand today are "noisy", meaning they're prone to errors when conducting quantum algorithms

We outline BQP as a superset of the P complexity class, but it also encapsulates a few NP class problems, and this is where we can express [Quantum Supremacy](https://en.wikipedia.org/wiki/Quantum_supremacy) or Quantum Advantage, the idea that a programmable quantum device can solve a problem in a feasible amount of time that a classical computer cannot.



## Noise

**Noise** occurs when our qubits change state in some manner. This can come from changes in the state like from $\left| + \right\rangle$ to $\left| 0 \right\rangle$ or changes in the phase of the qubit like from $\left| 1 \right\rangle$ to $i\left| 1 \right\rangle$

- A potential cause of noise can be from outside particles interacting with our qubit in Quantum Computers that must be kept at <mark style="background: #baf2ef;">near-absolute-zero</mark> temperatures



# Basics to Quantum Algorithms



Before we can jump right into the basics of QA's, there's a property of qubits we must explore, that being Phase.



## Phase & Interference

We work with phase in Quantum Computing similarly to how we work with it in **sound** or **alternating current** in the sense that we're using <u>constructive</u> and <u>destructive</u> interference to make certain outcomes more or less likely; the phase represents some angle that a qubit is currently "oscillating" at. This commonly could be $\pi$, $\frac {\pi}2$ or $\frac \pi 4$, but we can use any angle from $0$ to $2\pi$. 

- On the Bloch Sphere, this is why we have the $z$-axis
- In its equation, $\left| \psi \right\rangle = \cos(\frac {\theta}{2})\left| 0 \right\rangle + e^{i\phi}\sin(\frac {\theta}{2})\left| 1 \right\rangle$, it's why we have the Euler Identity: $e^{i\phi} = \cos(\phi) + i\sin(\phi)$



### Phase Kickback





## Oracle Algorithms

### What are Oracles?

We can think of oracles as black boxes of quantum gate operations; we don't necessarily know what's inside the box, but we can figure it out. The 'Archaic' definition of the word, oracle, tells us that, if we ask an oracle a question, we should get a response, however obscure or ambiguous.

Take the game 'Guess the Number' for example. You ask your friend 'Is it 50?' and they tell you 'Higher'. You go back and forth until you arrive at the number your friend was thinking of a.k.a. the concrete answer. The same thing happens here, but we're worried about what the oracle does.

Using an $N$ set of qubits, we can ask an oracle a question and get back some type of effect on the input set.



### Bernstein-Vazirani Oracle (Guess the secret code)



### Archimedes Oracle (How many secret codes are there?)



## Let get a bit more complex

### Deutsch-Jozsa





##### These will be optional put in

### Quantum Teleportation





### Superdense Codes



### BB84