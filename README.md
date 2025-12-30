# EMS741 - Deep Learning for Data and Image Analysis

A repository that contains tutorials, datasets and other resources for the EMS741 (Deep Learning for Data and Image Analysis) module at Queen Mary University of London.

## Teaching Team:

- Claire Villette (c.villette@qmul.ac.uk) - Module Organiser and Lecturer
- Shaheer U. Saeed (shaheer.saeed@qmul.ac.uk) - Lecturer
- TBD - Teaching Associate

## Code Requirements:

Tutorials, lab sessions and coursework all use Jupyter notebooks in [Google Colab](https://colab.research.google.com/). All ipynb files in this repository can be uploaded into Google Colab and accessed interactively. By default, all uploaded notebooks are saved into your Google Drive, so if you need to find one again, please refer to the correct Google Drive folder as opposed to uploading the same notebook again.

For any notebooks that you use as part of this module, please ensure that the first cell downloads the requisite data and installs the required python packages. Refer to the `intro_to_python` tutorial in the repository for further details. A minimal example is provided below:

```
!pip install torch tensorflow matplotlib nibabel
!wget -O data.zip https://github.com/s-sd/EMS741/raw/refs/heads/main/tutorials/intro_to_python/data.zip

import nibabel as nib
import numpy as np
import matplotlib.pyplot as plt
import os
```

## Deep Learning Python Packages:

For this module, you will be building neural networks using a specific python package. There are three major packages that are popular for deep learning in python, namely: `tensorflow`, `pytorch` and `jax`. They offer different levels of abstraction, in the following order from highest level to lowest level:

1) [`tensorflow` / `keras`](https://www.tensorflow.org/): offers a high-level interface for building neural networks (along with a lot of lower-level functionality, if desired); this package was quite popular for research purposes but is now being overtaken by the other two listed packages; if you are less familiar with python, we recommend this package.

2) [`pytorch`](https://pytorch.org/): offers a lower level of abstraction but remains accessible to users familiar with python; this is the most common deep leanring package today, in both research and industry; if you are comfortable with python and/ or willing to put in some extra effort to learn some basics, we recommend this package.

3) [`jax`](https://docs.jax.dev/en/latest/): this is the newest package and offers the lowest level of abstraction (i.e., you may have to code the specific behaviours of some types of layers etc.); this is growing rapidly in usage and lots of other packages that depend on jax are being released, which allow for higher levels of abstraction; if you are comfortable with python and want to explore the bleeding-edge you may use this package (however, specific support from the teaching team may be limited).

Please pick one of these packages for the entirety of this module, based on your experience with python or deep leanring. Skills learnt on one of these packages are easily transferred to another so you can always quickly learn the other two pacakges in your own time. 
