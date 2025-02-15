Data Transforms
===============

Data transforms are used to change the type or distribution of data variables.

This is a large umbrella of different techniques and they may be just as easily applied to input and output variables.

Recall that data may have one of a few types, such as numeric or categorical, with subtypes for each, such as integer and real-valued for numeric, and nominal, ordinal, and boolean for categorical.

* **Numeric Data Type:** Number values.
     * **Integer:** Integers with no fractional part.
     * **Real:** Floating point values.
* **Categorical Data Type:** Label values.
    * **Ordinal:** Labels with a rank ordering.
    * **Nominal:** Labels with no rank ordering.
    * **Boolean:** Values True and False.
    
The figure below provides an overview of this same breakdown of high-level data types.

.. figure:: ../_assets/nid/DataVariableTypes.png
   :alt: Overview of Data Variable Types
   :width: 90%
   
We may wish to convert a numeric variable to an ordinal variable in a process called discretization. Alternatively, we may encode a categorical variable as integers or boolean variables, required on most classification tasks.

* **Discretization Transform:** Encode a numeric variable as an ordinal variable.
* **Ordinal Transform:** Encode a categorical variable into an integer variable.
* **One-Hot Transform:** Encode a categorical variable into binary variables.

For real-valued numeric variables, the way they are represented in a computer means there is dramatically more resolution in the range 0-1 than in the broader range of the data type. As such, it may be desirable to scale variables to this range, called normalization. If the data has a Gaussian probability distribution, it may be more useful to shift the data to a standard Gaussian with a mean of zero and a standard deviation of one.

* **Normalization Transform:** Scale a variable to the range 0 and 1.
* **Standardization Transform:** Scale a variable to a standard Gaussian.

The probability distribution for numerical variables can be changed.

For example, if the distribution is nearly Gaussian, but is skewed or shifted, it can be made more Gaussian using a power transform. Alternatively, quantile transforms can be used to force a probability distribution, such as a uniform or Gaussian on a variable with an unusual natural distribution.

* **Power Transform:** Change the distribution of a variable to be more Gaussian.
* **Quantile Transform:** Impose a probability distribution such as uniform or Gaussian.

An important consideration with data transforms is that the operations are generally performed separately for each variable. As such, we may want to perform different operations on different variable types.

.. figure:: ../_assets/nid/DataTransforms.png
   :alt: Overview of Data Transforms
   :width: 90%

We may also want to use the transform on new data in the future. This can be achieved by saving the transform objects to file along with the final model trained on all available data.
