+++
title = "frequency and spatial filtering for periodic noise removal"
description = "python, pandas, numpy, scikit-learn, opencv. one of my favorite class assignments of all time. this was an assignment for my digital image processing course."
weight = 4

[extra]
local_image = "/projects/cropped_clown_dft.jpg"
+++

frequency and spatial filtering for periodic noise removal:

here we were tasked to use fourier transform on a signal. our signal is an image but to apply the fourier transform we have to note two things:

1. treat the entire image as one period.
2. we have to use the discrete fourier transform instead of continuous since image pixels `image[i][j]` can only be integers

**updated** : 09/19/2024

**todo**: provide visuals and finish explanation
