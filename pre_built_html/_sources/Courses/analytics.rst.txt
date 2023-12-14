Analytics 
++++++++++++++++++++++++++++++++++++++++++++++++++++



Prediction perfromance assestmet
=====================================================

OCD occurs whent you cant stop of thinking about something,
but i could i sure that i have OCD?, 
you can visit your professional health, and take several test to diagnose,
but what happens if the test is wrong? or what happend if the test said that not and
your thoughts are persistent!



imagine a similar situation with a major degree of certain, whichs means?
this means that there are a golden standard to diagnose, and you are testing a cheaper method, 
think in diagnose of covid-19 there are some situations

#. Test say **not** and i'm really **not have** covid-19
#. Test say **not** and i'm reall **have** covid-19
#. Test say **yes** and i'm really **have** covid-19
#. Test say **yes** and i'm really **dont have** covid-19



This could be summaries in:






Ok!, then how good fit this test?,  there are some metrics that i could study:

specificity
------------------------------------------------




sensitivity
--------------------------------------------------


Confusion Matrix

+---------------+---------------------+-----------------------+
|               |  Disease (Positive) | No-disease (Negative) |
+---------------+---------------------+-----------------------+
| Test Positive |  True Positive (TP) |  False Positive (FP)  |
+---------------+---------------------+-----------------------+
| Test Negative | False Negative (FN) |   True Negative (TN)  |
+---------------+---------------------+-----------------------+



Accuracy
---------------------------

.. warning:: 
    
    This measure is biased when there are unbalanced classes


is a unbiased measure of performance given that is affected by unbalanced classes.


.. math:: 
    :nowrap:

    \begin{equation}
        \text{Accuracy} = \frac{TP  + TN}{FP + FN + TP + FN}
    \end{equation}




 *Type I Error* and *False Positive Error*

.. math:: 
    :nowrap:

    \begin{equation}
        \text{Type 1} = \frac{FP}{TN + FP}
    \end{equation}

 
.. math:: 
    :nowrap:

    \begin{equation}
        \text{Type 2} = \frac{FN}{TP+FN}
    \end{equation}

For instance in bankruptcy is better have a error one or two?


We can extend to hypothesis testing.....