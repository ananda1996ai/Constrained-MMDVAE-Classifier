# The Denoising Classifier

The InfoVAE model uses MMD as an objective function replacing the original KL formulation. This comes from a natural derivation from the ELBO objective added with a mutual information constraint.

However, the interesting benefit of MMD over KL can be estimated from data sample points rather than prior distributions.

This allows for the MMD objective to be re-designed such that samples from a multi-class (2 or 3 class) dataset are represented in the latent space in a manner that distinct classes are mapped to distinct, pre-defined regions of the latent space. A distance based metric can be further used on the latent space to identify membership of a test sample to one of the classes. 
This allows for development of classifier models that are incredibly fast, and very robust to noise.

Thus, we can moniker them as **denoising classifiers** 😀

Here we demonstrate the model and it's functionality, and performance on a Sound Classification dataset. (MIMII: https://zenodo.org/record/3384388)

Currently the entire code is given in an .ipynb file, but a more modularised codebase will be committed shortly.

*This work was selected for best paper at a coporate whitepaper contest organised by Affine (Bengaluru, India).*

*Consider this work copyrighted to the owner of the repository.*
