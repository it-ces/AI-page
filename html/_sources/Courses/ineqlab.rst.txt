Inequality Measures
+++++++++++++++++++++++++++++++++++++++++




Introduction
====================================



Is important understand the uses of inequality Measures
to stuy the widespread of a disease over a territory,
the public 


Gini index
--------------------------------------------------






Entropy
====================================
Idea
============
Is a concept shanon offert a perspective...
comes from information theory...

$p_{i}$ the probability of occurnce
of the $i$ event, and $h(p_{i})$ is the value of of get the information that $i$ has been occur before than other one
known, not have value knonw with anticipation that occur a likyely event
that everyone wait.

if we have N events or in a 

.. math:: 
    :nowrap:

    \begin{equation}
    E = \sum p_{i} h(p_{i})
    \end{equation}

The entropy reach the maximun value with all the envets have the same probability.


# Bag model

We can think to $p_{i}$ as the probability of drawm from a bag with 'pesos' one 'peso' what is the 
probability of the 'peso' belong
to the $i$ person or unity.

.. math:: 
    :nowrap:

    \begin{equation}
    p_{i} = s_{i} = \frac{ x_{i}}{N \bar{y}}
    \end{equation}

the theil index will be the difference between the maximun theil possible and the real.

.. math:: 
    :nowrap:

    \begin{equation}
    T = \sum \frac{1}{N} h(\frac{1}{N}) - \sum s_{i}h(s_{i})
    \end{equation}

if we assmume that $h()$ is $-ln()$ we can 
take adwhile of that some properties
remember that a decresing function is good, 
and some logarithmic properties...

applying to the equations we have:

.. math:: 
    :nowrap:

    \begin{equation}
    T = \sum \frac{1}{N} -ln(\frac{1}{N}) - \sum s_{i} -ln(s_{i})
    \end{equation}


changing the value function we have:

.. math:: 
    :nowrap:

    \begin{equation}
    -ln(\frac{1}{N}) - \sum (\frac{x_{i}}{N \bar{y}})- ln(\frac{x_{i}}{N\bar{y}})
    \end{equation}

applying logartimic properties we have:

.. math:: 
    :nowrap:

    \begin{equation}
    T = -ln(\frac{1}{N}) - \sum \frac{x_{i}}{N\bar{y}} - ln(\frac{x_{i}}{\bar{y}}) - ln(\frac{1}{N})
    \end{equation}


therefore:


.. math:: 
    :nowrap:

    \begin{equation}
    T = \frac{1}{N} \sum \frac{x_{i}}{\bar{y}}ln(\frac{x_{i}}{\bar{y}})
    \end{equation}



#Restricted to $(0-1)$ theil index

Another point of view in SEN:

remeber that $\sum_{i}^{n} x_{i} = 1$.
$h(x) = ln(1/x) $ while $x$ be more improbably more value have$ (x) = \sum x_{i} log(\frac{1}{x_{i}})$ therefore
with $x_{i} = \frac{1}{n}$ then  $H(x) = log(n)$, remeber that we can write $log(n) = \sum x_{i} log(n)$, thus 


.. math:: 
    :nowrap:

    \begin{equation}
    T =  \sum x_{i}log(n) - \sum x_{i}log(\frac{1}{x_{i}})
    \end{equation}


We can acotate Theil index:

.. math:: 
    :nowrap:

    \begin{equation}
    \frac{T}{log(n)} = \frac{log(n) - H(x)}{log(n)}
    \end{equation}

if $H(x)$ is evenely distributed then $H(x) = log(n)$  if one person concentrate all then $H(x) = 0$. then wen a person concentrate all income $1*log(1/1) =0$.

therefore our index will be $1$ to perfect inequality and zero by uniform distribution.

code::

    def theil(array):
    Y = sum(array)
    N = len(array)
    relative = [y/Y for y in array]
    Theil = sum([y * math.log(y * N) for y in relative])/math.log(N)
    return Theil


# Discrete gini

.. math::
    :nowrap:

    \begin{equation}
    G = \frac{0.5 - B}{0.5}
    \end{equation}

Now we can see that


.. math::
    :nowrap:

    \begin{equation}
    G = 1 - 2B
    \end{equation}


.. math::
    :nowrap:

    \begin{equation}
    B = \sum \frac{(y_{i-1} + y_{i})}{2}*(N_{i} - N_{i-1})
    \end{equation}

the gini could be calculated with:

.. math::
    :nowrap:

    \begin{equation}
    G = 1 - \sum (y_{i-1} + y_{i}) * (N_{i} - N_{i-1})
    \end{equation}



code::
    def print(x)




codemaster
----------------



Theil index
------------------------------------------------

Theil index was defined by the economist Theil, and is based in information theory.... 


This lectuer is very important to constrait the gini index to a value.




The Theil index will be defined as:

the equations are important $h(X)=\sum_{i=1}^{N}x$

$$H(x)  = \sum_{i=1}^{N}$$


This is a excelent renderization, however never is enough..


Hamming distance
----------------------------------------------
.. _hammingdistance:


Hamming is a important distance 

Sometimes we need establish.. 

K-means
--------------------------------------------------------


The ideas of similarity also been linked to distance,
in a simple way, the way in which measure the distance is 
a fucking problem, given there are a lot of fucking distances...



Euclidean
-----------------------------------------------------------------------


Manhattan 
-----------------------------------------------------------------------



Another distance
--------------------------------------------------------------------------



We can test that there are a lot of distances.






