# Outliers Toolkit for Psychology, OTPsy

## Resume
In the last decades, lot of methods to detect outliers in a statistical distribution arised. Outliers are data point that are extremely distant from most of other data points.  
This package has the purpose to sum up the different method and to be able to used the different method without difficulty in psychology. The **particularity** is that it allows easily the computation of multiple columns testing.

For now, the package allows to detect outliers with a user-inputed distance with the method :
* IQR (IQR distance to median)
* Tukey (IQR distance from quartiles)
* Standard Deviation SD
* Recursive Standard Deviation rSD
* Median Absolute Distance MAD
* $S_n$ method
* Percentile
* Cut-off (reponse time under 80 ms for example)
* Identical response (for likert scale for example or behavioral performance)

The detection is made through the creation of an outliers object.

After the detection, they can be inspect through the inspect() method which returns a dataframe.
Outliers can be remove, winsorise or replace by na with the method `manage`

---

## Example

Imagine that you realise a study in which you want to explore the influence of art exposition on visual exploration of angry face (I don't know where this example came from, but it's sufficient). Thus, you collect data about the explored time of the painting scene, number of fixations of anger face (or another DV), score on depression and anxiety.
With this data, you want to control for different things :
* Does participants don't look at the scene ? 

## TODO

Visualisation through a dashboard is coming.  
Consistency between the different method for an outliers.
