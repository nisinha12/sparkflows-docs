Data Cleaning
=============

Data cleaning involves fixing systematic problems or errors in “messy” data.

The most useful data cleaning involves deep domain expertise and could involve identifying and addressing specific observations that may be incorrect.

There are many reasons data may have incorrect values, such as being mistyped, corrupted, duplicated, and so on. Domain expertise may allow obviously erroneous observations to be identified as they are different from what is expected, such as a person’s height of 200 feet.

Once messy, noisy, corrupt, or erroneous observations are identified, they can be addressed. This might involve removing a row or a column. Alternately, it might involve replacing observations with new values.

Nevertheless, there are general data cleaning operations that can be performed, such as:

* Using statistics to define normal data and identify outliers.
* Identifying columns that have the same value or no variance and removing them.
* Identifying duplicate rows of data and removing them.
* Marking empty values as missing.
* Imputing missing values using statistics or a learned model.
* Data cleaning is an operation that is typically performed first, prior to other data preparation operations.

.. figure:: ../_assets/nid/DataCleaning.png
   :alt: Overview of Data Cleaning
   :width: 90%
