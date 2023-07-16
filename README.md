# SVD-and-Its-Application
Image compression &amp; Denoise Image with SVD
# Outline
- Explain Vector
- Explain Eigenvector
- Explain Eigenvalue
- Combination of Eigenvector & Eigenvalue
- Explain SVD
# References: AI Viet Nam
## Vector:
- Vector is an object has both a magnitude and a direction.
- Vector is a matrix with single column or single row.
  + ![vector](https://drive.google.com/uc?export=view&id=1fdecoJYCHKGUwLPsU4filew6n6OuEb9P)
  + ![Relations of Vectors](https://drive.google.com/uc?export=view&id=1ltstLifSYZLwCNvpioZRsvk7w0Na_naL)
## Eigenvector
- A eigenvector v, is a non-zero vector that sastifies the following equation:
+ ![eigenvector](https://drive.google.com/uc?export=view&id=1pkJiIL5cT2tYnG5e14ZM72md48aok1eA)
+ Vector v is called eigenvector of matrix A if we multiply matrix A by vector v, the new vector (lamda)v does not change direction after the transformation
+ ![eigenvector](https://drive.google.com/uc?export=view&id=1WNch_kuC8UU1Q5oLpf7uA_L6EN6ZNSV-)
+ ![non eigenvector](https://drive.google.com/uc?export=view&id=1HL8dKJtkiynjMAE9VcuoY66TTq0jmn5p)
## Eigenvalue
- Eigenvalue tell us how much the eigenvector changes in size when mutiplied with the matrix
![Eigenvalue](https://drive.google.com/uc?export=view&id=1pkJiIL5cT2tYnG5e14ZM72md48aok1eA)
![Eigenvalue1](https://drive.google.com/uc?export=view&id=1aHBmFO5uTns9nnCN9UqI17TQTLPOkr9b)
- New column vector (lamda)v has same direction eigenvector.
- New column vector (lamda)v maybe either longer or shorter than eigenvector because of eigenvalue Lamda.
- Eigenvalue lamda might be negative. The direction of new vector is reversed but still on the same line
- We might find many eigenvectors of matrix A
- All vector with the same direction are actually eigenvector of matrix A
- ![eigenvalue2](https://drive.google.com/uc?export=view&id=16qb3EkNAx1UdWJ9MQ5bJZCAV-Y18oCbv)
## Combination of Eigenventor & Eigenvalue
![combination1](https://drive.google.com/uc?export=view&id=1vRLc39AjlANl-1WlMHuQWu3S5dyjplj-)
![combination2](https://drive.google.com/uc?export=view&id=1gPSlSm9cIHk2NJGPqYw83neqQM2X3lni)
![combination3](https://drive.google.com/uc?export=view&id=1ZyyNLPIWuU65NczQiL5yHc_GZuX7MZbh)
## Singular Value Decomposition
Since mathematics is just the art of assigning different names to the same concept, SVD is nothing more than decomposing vectors onto orthogonal axes.
- ![decompose](https://drive.google.com/uc?export=view&id=1gWGEsvZ0nzjBj9D65XSERkrHAVO1pE4o)
- Support u and v are vectors
  + Vector u decomposed into orthogonal components w1 and w2
  + Want to decompose u as: u = w1 + w2
- w1 is parallel to vector v and w1 is perpendicular/orthogonal to w2
- The vector component w1 is also called the projection of vector u onto vector v:
  + w1 = proj(v)(u) (projection of vector u onto vector v).
  + w2 = u - w1
### Decomposing a Vector into two Orthogonal Vectors
- ![decompose1](https://drive.google.com/uc?export=view&id=19ATaBgb3EnvE9HOlMRE_JYwWo-X-MJP6)
### Vector Projection
- ![decompose2](https://drive.google.com/uc?export=view&id=1OKdWmbqr4IQBqNL0QpoAXbyITLDWu8UJ)
### Extend this conclusion for handling a matrix (a bunch of vectors)
- ![decompose3](https://drive.google.com/uc?export=view&id=1hq8w4HS70kljgc9JOVBewA-IPbfZniBo)
### Recall Vector Projection
- ![recall1](https://drive.google.com/uc?export=view&id=1EH6UZRPWenCGwrjG0WY8j1QuEn77buQ7)
- ![recall2](https://drive.google.com/uc?export=view&id=1MHEBlBNnjWhbvYdWAOipuKBaBxdVvXeE)
- ![recall3](https://drive.google.com/uc?export=view&id=1LlLrq4gFY3pKRKXSfI6kMNaI7vdYt4eP)
- Extend to more than 1 vectors.
- ![recall4](https://drive.google.com/uc?export=view&id=1AZUfC5WdT4Je-h1_jJVdbOzFcO16ZOcI)
- Generalize to any number of points and dimensions
- ![recall5](https://drive.google.com/uc?export=view&id=1GrOo9VaNc724HjUOMX1gU9C0RgTPwKAT)
- ![recall 6](https://drive.google.com/uc?export=view&id=1s9M_gWTGGlpDFRoH16F7h_xmnD_e2Xhp)
- Any set of vectors (A) can be expressed in terms of their lengths of projections (S) on some set of orthogonal axes (V).
- ![recall6](https://drive.google.com/uc?export=view&id=1PC87haQoTb33YJomDD8Ynn8Tg1IpiHyt)
### We are here!
![wearehere](https://drive.google.com/uc?export=view&id=1jPybrE2IZG1WgrqVfsObdPv_VNy58ZNN)
### Convention SVD
![ConventionSVD](https://drive.google.com/uc?export=view&id=1Mx5fTM013FSY_dR4-Z0diMB68gA1vjac)
### Keep going on decomposing S
![S](https://drive.google.com/uc?export=view&id=1iotBOirO4cnlMpEB4MiHuA3aJUNcYckD)
###
![Sdecompose1](https://drive.google.com/uc?export=view&id=1SkFzDqnx5iI3ChqBr0ancZneqF7QHwJM)
- Normalize these comlumn vectors to make them of unit length
- Dividing each column vector by its magnitude, but in matrix form
  + ![Sdecompose2](https://drive.google.com/uc?export=view&id=1drf9N6FeOi74hIK3a2-755o_vbotSm0Z)
  + ![Sdecompose3](https://drive.google.com/uc?export=view&id=1mLdiSuvnYoxzmI-QRpV6AjJHMCRQdKmC)
### S - Explanation
![WhyS](https://drive.google.com/uc?export=view&id=1DFqpXS651c0ScSpuFF5qbVzmxEx_iYqh)
### Sigma - Explanation
- Sigma determines most points (decomposed vector) are closer to v1 or v2.
![WhySigma](https://drive.google.com/uc?export=view&id=1uw97ldQHdoPdSBE4ZSVuo4taVEsGauLb)
## Another Approaching SVD (mapping to Eigenvector / Eigenvalue)
- ![AnotherApproaching](https://drive.google.com/uc?export=view&id=1VioU57h8CGH4zxJZeAqhptEItuJgJKqc)
- For Example:
- ![Example](https://drive.google.com/uc?export=view&id=1KQ3cG8zy6lVRVxfDCYeJPCmmTa_0ABTw)
