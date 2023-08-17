# bayes_python

1. Testing bayes' theorem applications to strain screening (bayesian T-testing)
2. Bayesian forcasting and dynamic modelling of a bioreactor for parameter fits/estimation and uncertainty quantification

Installation & Python Environment:

Follow the pymc3 install instructions using conda

I tried going around this and just using pip but there is a c++ compiler dependency that
was more easily managed with conda and Intel's MKL (optimized linear algebra library) was better
managed through conda. All came in with the pymc install. 

The install got messy when I tried to set the Theano and/or PyTensor
BLAS to look at MKL. It was stuck on the Numpy C-API BLAS that was slow, ~5 minutes to run 4 chains + 1000 samples
in the MCMC.

