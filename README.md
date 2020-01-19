# Learning Decision Boundaries #

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/MovingImage" property="dct:title" rel="dct:type">Decision Boundaries Animations</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://twitter.com/ryanpholbrook" property="cc:attributionName" rel="cc:attributionURL">Ryan Holbrook</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/ryanholbrook/decision-boundaries-animations" rel="dct:source">https://github.com/ryanholbrook/decision-boundaries-animations</a>.

This repository contains GIF animations of classifiers learning a decision rule. We can visualize the rule a classifier learns as a decision boundary separating the features of each class. In the animations, the *optimal* decision boundary is drawn with a dashed line. In a sense, the "goal" of a classifier is to fit a curve to this optimal boundary.

The animations depict a binary classification problem over two distributions. A `mvn` in the filename indicates the features of each class are distributed normally; a `mix` in the filename indicates the features of each class are distributed as a mixture of normal distributions.

The animations were created in R, using the `gganimate` package.

* TODO - List classifier packages and cite.

----

# Citations #

1.  Thomas Lin Pedersen and David Robinson (2019). gganimate: A Grammar
    of Animated Graphics. R package version 1.0.4.
    https://CRAN.R-project.org/package=gganimate
