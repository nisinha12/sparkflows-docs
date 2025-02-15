Feature Engineering
===================

Feature engineering refers to the process of creating new input variables from the available data.

Engineering new features is highly specific to your data and data types. As such, it often requires the collaboration of a subject matter expert to help identify new features that could be constructed from the data.

This specialization makes it a challenging topic to generalize to general methods.

Nevertheless, there are some techniques that can be reused, such as:

* Adding a boolean flag variable for some state.
* Adding a group or global summary statistic, such as a mean.
* Adding new variables for each component of a compound variable, such as a date-time.

A popular approach drawn from statistics is to create copies of numerical input variables that have been changed with a simple mathematical operation, such as raising them to a power or multiplied with other input variables, referred to as polynomial features.

* **Polynomial Transform:** Create copies of numerical input variables that are raised to a power.
The theme of feature engineering is to add broader context to a single observation or decompose a complex variable, both in an effort to provide a more straightforward perspective on the input data.

I like to think of feature engineering as a type of data transform, although it would be just as reasonable to think of data transforms as a type of feature engineering.
