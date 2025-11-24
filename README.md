# Herbivore Bite Rates on Moorea Reefs (2010)

To understand the interaction between herbivorous fish species and coral reefs in Moʻorea, we will run statistical model to determine how the morphology and environment affect the number of bite counts on a coral reef.

### Hypothesis

How is the herbivore grazing bite counts related to fish size, species, depth, and substrate?

**Null Hypothesis:** Either size, species, depth, or substrate have no effect on bite count.

**Alternative Hypothesis:** A predictor/predictors have an effect on bite count.

Since our response variable, Total Bites, is discrete count data, we will use a **Negative Binomial** statistical model.

### Poisson model notation:

$$
\begin{align}
\text{BiteCount} &\sim NegativeBinomial(\lambda) \\
log(\lambda) &= \beta_0 + \beta_1 \text{Size} + \beta_2 \text{Species} + \beta_3\text{Size}(Species)  + \beta_4 \text{Depth} + \beta_5 \text{Substrate}
\end{align}
$$

### Hypothesis in Statistical Notation

$$H_0: \beta_1 = 0 \\
  H_A: \beta_1 \neq 0$$
