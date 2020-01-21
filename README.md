# Learning Decision Boundaries #

This repository contains GIF animations of classifiers learning a decision rule. We can visualize the rule a classifier learns as a decision boundary separating the features of each class. In the animations, the *optimal* decision boundary is drawn with a dashed line. In a sense, the "goal" of a classifier is to fit a curve to this optimal boundary.

The animations depict a binary classification problem over two distributions. A `mvn` in the filename indicates the features of each class are distributed normally; a `mix` in the filename indicates the features of each class are distributed as a mixture of normal distributions.

The animations were created in R, using the `{gganimate}` package. The classifiers illustrated are:

+ [Extreme Learning Machine](https://en.wikipedia.org/wiki/Extreme_learning_machine) with `{elmNNRcpp::elm_train}`
+ [Gaussian Process](https://en.wikipedia.org/wiki/Kriging) with `{kernlab::gausspr}`
+ [Generalized Additive Model](https://en.wikipedia.org/wiki/Generalized_additive_model) with `{mgcv::gam}`
+ [Generalized Linear Model](https://en.wikipedia.org/wiki/Generalized_linear_model) with `{stats::glm}`
+ [k-Nearest Neighbors](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm) with `{class::knn}`
+ [Multivariate Adaptive Regression Spline](https://en.wikipedia.org/wiki/Multivariate_adaptive_regression_spline) with `{earth::earth}`
+ [Mixture Discriminant Analysis](https://web.stanford.edu/~hastie/TALKS/mfpda.pdf) with `{mda::mda}`
+ [Naive Bayes Classifier](https://en.wikipedia.org/wiki/Naive_Bayes_classifier) with `{naivebayes::naive_bayes}`
+ [Feedforward Neural Network](https://en.wikipedia.org/wiki/Feedforward_neural_network) with `{nnet::nnet}`
+ [Polynomial MARS](http://kooperberg.fhcrc.org/monopdf/mono.html) with `{polspline::polymars}`
+ [Boosted P-Splines](https://en.wikipedia.org/wiki/B-spline) with `{mboost::mboost}`
+ [Quadratic Discriminant Analysis](https://en.wikipedia.org/wiki/Quadratic_classifier) with `{MASS::qda}`
+ [Random Forest](https://en.wikipedia.org/wiki/Random_forest) with `{ranger::ranger}`
+ [Decision Tree](https://en.wikipedia.org/wiki/Decision_tree_learning) with `{rpart::rpart}`
+ [Support Vector Machine](https://en.wikipedia.org/wiki/Support-vector_machine) using [RBF kernel](https://en.wikipedia.org/wiki/Radial_basis_function_kernel) with `{kernlab::ksvm}`
+ [Gradient Boosting](https://en.wikipedia.org/wiki/Gradient_boosting) with `{xgboost::xgboost}`

## Citations ##

+  Thomas Lin Pedersen and David Robinson (2019). gganimate: A Grammar
   of Animated Graphics. R package version 1.0.4.
   https://CRAN.R-project.org/package=gganimate
+  H. Wickham. ggplot2: Elegant Graphics for Data Analysis.
   Springer-Verlag New York, 2016.
+  Lampros Mouselimis and Alberto Gosso (2018). elmNNRcpp: The Extreme
   Learning Machine Algorithm. R package version 1.0.1.
   https://CRAN.R-project.org/package=elmNNRcpp
+  R Core Team (2018). R: A language and environment for statistical
   computing. R Foundation for Statistical Computing, Vienna, Austria.
   URL https://www.R-project.org/.
+  Wood, S.N. (2017) Generalized Additive Models: An Introduction with R
   (2nd edition). Chapman and Hall/CRC.
+  Venables, W. N. & Ripley, B. D. (2002) Modern Applied Statistics with
   S. Fourth Edition. Springer, New York. ISBN 0-387-95457-0
+  Stephen Milborrow. Derived from mda:mars by Trevor Hastie and Rob
   Tibshirani. Uses Alan Miller's Fortran utilities with Thomas Lumley's
   leaps wrapper. (2019). earth: Multivariate Adaptive Regression
   Splines. R package version 5.1.2.
   https://CRAN.R-project.org/package=earth
+  Venables, W. N. & Ripley, B. D. (2002) Modern Applied Statistics with
   S. Fourth Edition. Springer, New York. ISBN 0-387-95457-0
+  Charles Kooperberg (2019). polspline: Polynomial Spline Routines. R
   package version 1.1.17. https://CRAN.R-project.org/package=polspline
+  Marvin N. Wright, Andreas Ziegler (2017). ranger: A Fast
   Implementation of Random Forests for High Dimensional Data in C++ and
   R. Journal of Statistical Software, 77(1), 1-17.
   doi:10.18637/jss.v077.i01
+  Terry Therneau and Beth Atkinson (2019). rpart: Recursive
   Partitioning and Regression Trees. R package version 4.1-15.
   https://CRAN.R-project.org/package=rpart
+  Alexandros Karatzoglou, Alex Smola, Kurt Hornik, Achim Zeileis
   (2004). kernlab - An S4 Package for Kernel Methods in R. Journal of
   Statistical Software 11(9), 1-20. URL
   http://www.jstatsoft.org/v11/i09/
+  Tianqi Chen, Tong He, Michael Benesty, Vadim Khotilovich, Yuan Tang,
   Hyunsu Cho, Kailong Chen, Rory Mitchell, Ignacio Cano, Tianyi Zhou,
   Mu Li, Junyuan Xie, Min Lin, Yifeng Geng and Yutian Li (2019).
   xgboost: Extreme Gradient Boosting. R package version 0.90.0.2.
   https://CRAN.R-project.org/package=xgboost

## License ##

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/MovingImage" property="dct:title" rel="dct:type">Decision Boundaries Animations</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/ryanpholbrook" property="cc:attributionName" rel="cc:attributionURL">Ryan Holbrook</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/ryanholbrook/decision-boundaries-animations" rel="dct:source">https://github.com/ryanholbrook/decision-boundaries-animations</a>.
