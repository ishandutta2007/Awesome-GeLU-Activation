# Gaussian Error Linear Unit (GELU)

The **Gaussian Error Linear Unit (GELU)** is a high-performance activation function that weights inputs by their probability under a Gaussian distribution.

## Mathematical Definition
$$\text{GELU}(x) = x \cdot \Phi(x)$$
where $\Phi(x)$ is the Cumulative Distribution Function (CDF) of the standard normal distribution.

## Visualization
```mermaid
xychart-beta
    title "GELU Activation Function (Approximation)"
    x-axis [-3, -2, -1, 0, 1, 2, 3]
    y-axis "f(x)" [-0.2, 3]
    line [-0.004, -0.045, -0.158, 0, 0.841, 1.954, 2.996]
```

## History & Origins
- **First Proposed:** 2016 by Dan Hendrycks and Kevin Gimpel in [Gaussian Error Linear Units (GELUs)](https://arxiv.org/abs/1606.08415).
- **First Major Use:** 
  - **BERT** (2018): Google used GELU as the default activation in the BERT encoder.
  - **GPT-2** (2019): OpenAI standardized GELU for their generative transformer models.

## Characteristics
- **Smoothness:** Unlike ReLU, GELU is smoothly differentiable everywhere.
- **Non-monotonicity:** It has a small negative "dip," which helps with gradient flow for values near zero.
- **Stochastic Interpretation:** It can be seen as a deterministic version of dropout.

[Back to README](../README.md)
