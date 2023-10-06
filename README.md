Oil and gas fields need to be forecasted. Before the subject of reservoir engineering (mainly the Decline Curve Analysis, or DCA) came as knowledge and practice, people still did not have the notion that oil and gas reservoirs could be made predictable. No longer until J. J. Arps published his "Analysis of Decline Curves" to AIME in 1945, it is now the duty of every reservoir engineer to be able to forecast the future production rate of their wells in the field.

Before Arps classified three decline curve types, actually there were many engineers as early as in 1908 who were analyzing decline curves. In 1924, Cutler discovered the hyperbolic decline on a log-log paper for his analysis. One year later, Larkey proposed the use of least squares to extrapolate decline curves. Both contributed the basis to Arps.

DCA has been general knowledge and practice nowadays to forecast future production. Additionally, the popularity of scientific computing gives more promises to engineers so that we can do rigorous analysis much faster using programs. This objective of this article is to share a tutorial on doing DCA using Python.

Three Decline Curve Types of Arps
Arps (1945) formulated the general decline function for oil and gas wells as follows:

No alt text provided for this image
Where q is the production rate (STB/day or SCF/day), t is the time (days), qi is the initial production rate (same unit as q), di is the initial decline rate (same unit as q), and b is the decline exponent. This decline function is known as the hyperbolic decline function.

Based on the value of b in the function, he then classified the decline curves into three types:

* The exponential decline has b equals 0.
* The harmonic decline has b equals 1.
* The hyperbolic decline has b ranges between 0 and 1.

## Limitations of Arps' Decline Curve
Arps formulated his three type-curves based on evidence in the late-stage of the field life. If we recall about types of flow behavior in a reservoir, the flow in this stage behaves in a boundary-dominated condition, or often called as the pseudo-steady flow at a time when the reservoir approaches the boundary. In the early life of the field, the flow in the reservoir behaves in a transient condition. If we recall why we could get the b value larger than 1, this could mean that the flow inside still behaves transiently.

In other words, Arps' decline curves give more acceptable forecasts only in the later life of the field. 30 years later, Fetkovich (1980) and Carter (1985) proposed other type curves that extend the Arps' type to be capable in the analysis of the early life of the field. According to Lee and Wattenbarger (1996), the main difference between Arps' and both of the proposed type curves is that Arps' decline is based on empirical evidence, unlike both Fetkovich and Carter are based on theoretical. Therefore, both methods are generally more applicable.

References
Lee, J., R. A. Wattenbarger. (1996). Gas Reservoir Engineering: SPE Textbook Series Vol. 5. Society of Petroleum Engineers

Towler, B. F. (2002). Fundamental Principles of Reservoir Engineering: SPE Textbook Series Vol. 8. Society of Petroleum Engineers

Norwegian Petroleum Directorate website about Norne Field information

https://www.linkedin.com/pulse/decline-curve-analysis-python-yohanes-nuwara/
