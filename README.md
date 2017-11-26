## Overview

simNum is a number simulator for Normal, Poisson or Binomial distributions.

## Code Example

```
import simNum

d = simNum.simDist(10,'normal')

print(d)
```

## Dependencies

[NumPy](https://github.com/numpy/numpy)

## Installation

This package can be installed using pip by simply running the line of code below in your terminal. Note you may need to add sudo to the beggining depending on your permissions setup.

```
pip install simNum
```

Alternatively if you'd like to install manually you can follow the steps below.

1. Download the package [here](https://pypi.python.org/pypi/simNum/2.1)
2. Unzip the file
3. Change directory in your terminal to the directory containing the downloaded setup.py file
4. Type `python setup.py install` and hit press return

## Documentation

The package only contains one function `simDist()` which takes the following parameters:

__simNum.simDist__ _(samples,distribution,mean=0,stddev=1,lamb=1,trials=None,probability=None)_
* __samples__ _: int_

    The number of samples required.

* __distribution__ _: str_

    Specifies the type of distribution 'normal', 'poisson' or 'binomial'.
    
* __stddev__ _: float_

    Standard deviation (spread or “width”) of the distribution.

* __lamb__ _: float_

    This parameter is only used for the poisson distribution. Expectation of interval, should be >= 0. A sequence of expectation intervals must be broadcastable over the requested size.

* __trials__ _: int_

    This parameter is only used for the binomial distribution. Parameter of the distribution, >= 0. Floats are also accepted, but they will be truncated to integers.
    
* __probability__ _: float_

    This parameter is only used for the binomial distribution. Parameter of the distribution, >= 0 and <=1.
    
Further documention for the parameters associated with each distribution can be found here: [normal](https://docs.scipy.org/doc/numpy-1.13.0/reference/generated/numpy.random.normal.html), [binomial](https://docs.scipy.org/doc/numpy-1.13.0/reference/generated/numpy.random.binomial.html), [poisson](https://docs.scipy.org/doc/numpy-1.13.0/reference/generated/numpy.random.poisson.html).

## Contributors

I highly doubt anyone will want to contribute to this project but please feel free!

## License

[MIT](https://github.com/Roundy123/simNum/blob/master/LICENSE.txt)
