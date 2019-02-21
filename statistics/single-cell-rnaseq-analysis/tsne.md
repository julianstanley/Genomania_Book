# tSNE



**What is tSNE?**

![](https://lh4.googleusercontent.com/CmjWpWwtzgGpl1xUqV7RDXk471jxLprM-LGv-vtpaV-UYDvGIVPHrKJx3nQzk_Cyl5PKVSi_DyxqCpuhuNaVCwXJJNX054D4Qein7c5uGUkaQNhaoPeR7G3IqKihySiExwCYnzvYZwZ3uQ8I)

* Just a way to visualize high-dimensional data. In the case of single cell sequencing, we have say 10,000 cells, each with say expression of 25,000 transcripts. So that’s a 10,000 X 25,000 matrix, which we can’t plot in a 2D graph.
  * That basic problem can be solved by different methods, like Principal Component Analysis \(PCA\) or diffusion maps \(DM\).
  * tSNE is different because:
    * \(1\) It is an iterative machine learning algorithm, so it can produce different results each time it runs
    * \(2\) Rather than just plotting the points, tSNE explicitly tries to group points, making it a popular choice for single-cell group classifications.  

### Videos!

{% embed url="https://www.youtube.com/watch?v=NEaUSP4YerM" %}



