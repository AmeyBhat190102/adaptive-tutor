# Calculus

## Introduction
Calculus is the branch of mathematics that studies continuous change. It has two main branches: **differential calculus** (rates of change) and **integral calculus** (accumulation). Both are connected by the **Fundamental Theorem of Calculus**.

## Limits

### What is a Limit?
A limit describes the value a function approaches as the input approaches some value.

**Notation:** lim(x→a) f(x) = L means "as x approaches a, f(x) approaches L"

### Evaluating Limits
**Direct substitution** (when the function is continuous at that point):
- lim(x→3) (x² + 1) = 3² + 1 = 10

**Factoring** (when direct substitution gives 0/0):
- lim(x→2) (x² - 4)/(x - 2) = lim(x→2) (x+2)(x-2)/(x-2) = lim(x→2) (x+2) = 4

### One-sided Limits
- Left-hand limit: lim(x→a⁻) f(x) — approaching from the left
- Right-hand limit: lim(x→a⁺) f(x) — approaching from the right
- A limit exists only if both one-sided limits are equal

### Limits at Infinity
- lim(x→∞) 1/x = 0
- lim(x→∞) (3x² + 2x)/(x²) = 3

## Derivatives

### What is a Derivative?
The derivative of a function f(x) represents the **instantaneous rate of change** of f at any point x. Geometrically, it is the slope of the tangent line to the curve at that point.

**Definition (first principles):**
f'(x) = lim(h→0) [f(x+h) - f(x)] / h

### Differentiation Rules

**Power Rule:** d/dx[xⁿ] = nxⁿ⁻¹
- d/dx[x³] = 3x²
- d/dx[x⁵] = 5x⁴

**Constant Rule:** d/dx[c] = 0

**Constant Multiple Rule:** d/dx[cf(x)] = c·f'(x)

**Sum/Difference Rule:** d/dx[f(x) ± g(x)] = f'(x) ± g'(x)

**Product Rule:** d/dx[f(x)·g(x)] = f'(x)g(x) + f(x)g'(x)

**Quotient Rule:** d/dx[f(x)/g(x)] = [f'(x)g(x) - f(x)g'(x)] / [g(x)]²

**Chain Rule:** d/dx[f(g(x))] = f'(g(x))·g'(x)

### Derivatives of Common Functions
- d/dx[sin x] = cos x
- d/dx[cos x] = -sin x
- d/dx[eˣ] = eˣ
- d/dx[ln x] = 1/x

### Applications of Derivatives

**Finding slope of a tangent:**
f(x) = x² + 3x, find slope at x = 2
f'(x) = 2x + 3
f'(2) = 2(2) + 3 = 7

**Finding turning points (maxima/minima):**
1. Set f'(x) = 0 and solve for x (critical points)
2. Use second derivative test: if f''(x) > 0 → minimum; f''(x) < 0 → maximum

**Velocity and acceleration:**
If s(t) is position, then:
- v(t) = s'(t) — velocity (rate of change of position)
- a(t) = v'(t) = s''(t) — acceleration (rate of change of velocity)

## Integrals

### What is an Integral?
Integration is the reverse of differentiation. It calculates the **area under a curve** between two points, or finds a function from its derivative.

### Indefinite Integrals (Antiderivatives)
∫f(x)dx = F(x) + C, where F'(x) = f(x) and C is the constant of integration

**Power Rule for Integration:** ∫xⁿdx = xⁿ⁺¹/(n+1) + C (where n ≠ -1)
- ∫x²dx = x³/3 + C
- ∫x⁴dx = x⁵/5 + C

**Common Integrals:**
- ∫cos x dx = sin x + C
- ∫sin x dx = -cos x + C
- ∫eˣ dx = eˣ + C
- ∫(1/x) dx = ln|x| + C

### Definite Integrals
∫[a to b] f(x)dx = F(b) - F(a)

This gives the net area between the curve and the x-axis from x = a to x = b.

**Example:** ∫[1 to 3] x² dx
= [x³/3] from 1 to 3
= 3³/3 - 1³/3
= 9 - 1/3
= 26/3

### The Fundamental Theorem of Calculus
Connects differentiation and integration:

**Part 1:** If F(x) = ∫[a to x] f(t)dt, then F'(x) = f(x)

**Part 2:** ∫[a to b] f(x)dx = F(b) - F(a), where F is any antiderivative of f

### Applications of Integration
- Area between curves: ∫[a to b] [f(x) - g(x)]dx
- Volume of revolution (disk method): π∫[a to b] [f(x)]² dx
- Total distance from velocity: ∫|v(t)|dt
- Accumulated change: if f'(x) is rate of change, ∫f'(x)dx gives total change
