# Introductionn

We are working through the karpathy lectures on neural networks (namely the introductory one and the new one on gpt-2).

## Building micrograd

Micrograd is everything you need to build neural networks, everything else is just efficiency (not that it is any less important). So what is micrograd? It is just a simple autograd implementation allowing for forward and backward passes (backpropagation essentially).

## Taking derivative from scratch

Suppose that $f(x) = 3x^2 - 4x + 5$ such that $f(3) = 20$.

The derivative is calculated as: $f'(x = a) = \lim_{h \to 0}\frac{f(a + h) - f(a)}{h}$.

**Backprop**: we will take the derivative of the result wrt certain leaf nodes (weights) and not wrt others (obviously wont take against the data). And, backpropagation is dependent on chain rule.

It is interesting how the intuition for chain rule is essentially a fork from physics.