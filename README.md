# Geopandas-Mask-Creator
 Automatically create masks for use with non-rectangular spatial data in Geopandas

<br /><br /><br />
An example use case is shown below.

![Example](Example_output_with_and_without_mask.png)


It works by calculating the minimum width of buffer required to __guarantee__ coverage of the plot. This is then plotted on the same axis as the original data acting as a mask. 
<br /><br />
A geometric overlay is performed after the buffer is created to ensure any area with data will not be masked. This prevents the danger of two disjointed but nearby areas of data masking one another. 
<br /><br />
An example of how the buffer is created is shown below. 

![Example](Automated_width_of_buffer_created.png)
