# SiLU (Swish)

**SiLU** (Sigmoid-weighted Linear Unit), also known as **Swish**, is a smooth, non-monotonic activation function discovered through automated search.

## Mathematical Definition
$$f(x) = x \cdot \sigma(x) = \frac{x}{1 + e^{-x}}$$

## Visualization
```mermaid
xychart-beta
    title "SiLU / Swish Activation Function"
    x-axis [-4, -2, 0, 2, 4]
    y-axis "f(x)" [-0.3, 4]
    line [-0.07, -0.24, 0, 1.76, 3.92]
```

## History & Origins
- **First Proposed:** 
  - **SiLU:** 2017 by Elfwing et al. in [Sigmoid-Weighted Linear Units for Deep Reinforcement Learning](https://arxiv.org/abs/1702.03118).
  - **Swish:** 2017 by Ramachandran et al. (Google Brain) in [Searching for Activation Functions](https://arxiv.org/abs/1710.05941).
- **First Major Use:** 
  - **EfficientNet** (2019): Used extensively in the MBConv blocks, contributing to state-of-the-art accuracy/efficiency.

## Characteristics
- **Lower Bound:** It is bounded below but unbounded above.
- **Smoothness:** Provides a smoother transition than ReLU.

[Back to README](../README.md)
