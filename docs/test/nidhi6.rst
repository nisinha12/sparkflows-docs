Dimensionality Reduction
------------------------

The number of input features for a dataset may be considered the dimensionality of the data.

For example, two input variables together can define a two-dimensional area where each row of data defines a point in that space. This idea can then be scaled to any number of input variables to create large multi-dimensional hyper-volumes.

The problem is, the more dimensions this space has (e.g. the more input variables), the more likely it is that the dataset represents a very sparse and likely unrepresentative sampling of that space. This is referred to as the curse of dimensionality.

This motivates feature selection, although an alternative to feature selection is to create a projection of the data into a lower-dimensional space that still preserves the most important properties of the original data.

This is referred to generally as dimensionality reduction and provides an alternative to feature selection. Unlike feature selection, the variables in the projected data are not directly related to the original input variables, making the projection difficult to interpret.

The most common approach to dimensionality reduction is to use a matrix factorization technique:

* Principal Component Analysis (PCA)
* Singular Value Decomposition (SVD)

The main impact of these techniques is that they remove linear dependencies between input variables, e.g. correlated variables.

Other approaches exist that discover a lower dimensionality reduction. We might refer to these as model-based methods such as LDA and perhaps autoencoders.

* Linear Discriminant Analysis (LDA)

Sometimes manifold learning algorithms can also be used, such as Kohonen self-organizing maps and t-SNE.

.. figure:: ../_assets/nid/DimensionalityReduction.png
   :alt: Overview of Dimensionality Reduction Techniques 
   :width: 90%
   
