Export_to_XLSX is a script that can take all the data files in a folder, extracting the frequency, real impedance, and imaginary impedance and calculate all the impedance spectroscopy parameters (IS) and tau 
values for each sample.  There is a peak finder as well to find maxima in the values for M'', Z'', and Tan delta based on number and a stastic of nearest neighbor values to reduce or eliminate outlying data points.
Default values for sample thickness and electrode area are included, but individual values can be used with some modification, this will loop through all the files and create one XLSX for each data file.

This code was written with AI assistance to simply extracting electrochemical data without time consuming work with factory software from different instruments, or expensive software bundles.   The spreadsheet format
should simplify data management if not using python, and also reduces any calculations dowstream for large data sets as this is pre-calculated for plotting later.

Originally this was written to extract from Solartron 1260 legacy instrumentation, but has shown adaptable to other hardware such as Parstat and NOVO.

Once data is exported to XLSX, other scripts were weritten to manage the data in different ways for the various types of plots for full parameterization.

Script 2 (Characterization) creates autoscaled plots of Nyquist, Modulus (bode) (M'' vs frequency), phase angle (Phi), and admittance (Y),  Bode (Z'' vs frequency), complex modulus (M'v M''), Tan delta vs frequency, 
and Permittivity (real and imaginary vs frequency. This way the user can view all the data in one go in a 2X2 plot of data to see how it looks, and which graphs might be more intersting for a closer look. Each plot 
can be saved manually.  Also included here are a 3D modulus plot, and 3D impedance plot (Z', Z'' or M', M'' vs frequency in a 3 dimensional X,Y,Z plot) for closer inspection.  THIS IS NOT A WATERFALL PLOT but this could be done easily also. The 3D plot.

Script 3


