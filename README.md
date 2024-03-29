## Dynamic Model of Infectious Diseases

Python implementation of SI, SIR, SIS SEIR.

$N$-population

$i=I/N$ - infection ration

$s=S/N$ - susceptible ration

$r=R/N$ - removed ration

+ **SI model**
  
  [ S ] -- $\lambda$ --> [ I ]

  $\frac{di}{dt} = \lambda i (1-i)$
  
  ![SI](https://github.com/XuelongSun/Dynamic-Model-of-Infectious-Diseases/blob/master/results/SI.png)

+ **SIS model**
  
  [ S ] -- $\lambda$ --> [ I ]

  [ S ] <-- $\gamma$ -- [ I ]

  $\frac{di}{dt} = \lambda i (1-i) - \gamma i$
  
  ![SIS](https://github.com/XuelongSun/Dynamic-Model-of-Infectious-Diseases/blob/master/results/SIS.png)

+ **SIR model**

  [ S ] -- $\lambda$ --> [ I ] -- $\gamma$ --> [R]

  $\frac{ds}{dt} = -\lambda i s$

  $\frac{di}{dt} = \lambda i s - \gamma i$
  
  $\frac{dr}{dt} = \gamma i$

  ![SIR](https://github.com/XuelongSun/Dynamic-Model-of-Infectious-Diseases/blob/master/results/SIR.png)

+ **SEIR model**

  [ S ] -- $\lambda$ -->[ E ]-- $\sigma$ --> [ I ] -- $\gamma$ --> [R]

  $\frac{ds}{dt} = -\lambda i s$

  $\frac{de}{dt} = \lambda i s - \sigma e$

  $\frac{di}{dt} = \sigma e - \gamma i$
  
  $\frac{dr}{dt} = \gamma i$

  ![SEIR](https://github.com/XuelongSun/Dynamic-Model-of-Infectious-Diseases/blob/master/results/SIRE.png)
