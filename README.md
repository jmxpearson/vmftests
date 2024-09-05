# von Mises-Fisher experiments

Not much to document for now. The key integration test is in `vMF_inference.ipynb`, which constructs a simple 
dataset and verifies that we can learn the power spectrum via Sequential Monte Carlo. 

The implementation of SMC in that notebook is _not_ optimized. Individual functions are in JAX, but the 
entire training loop should be converted into a single `scan`.
