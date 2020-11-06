# data-collection-xlsx
This project contains an example excel file with VBA script to automatically generate graphs to aid in data analysis.

This excel file is for collecting data using a scale connected to a computer (with either a COM port reader such as PuTTY or proprietary software included with the scale) when collecting permeate from a dead-end cell filtration setup, specifically for Reverse Osmosis applications, the removal of NaCl from water.

How to use:

For pure DI water:

1. Either collect the data directly into the excel file in the 'Mass' column or a text file and copy and paste after the experiment is complete.
2. Once the raw data is in the file, add the effective filtration area for the dead-end cell, the pressure used for the experiment, and any relevant notes.
3. Adjust the 'Time' column so that each entry in the 'Mass' column has a corresponding time value. Make sure that the 'Time' column does not have any extra values where there is not a matching mass value or the macro will throw an error.
4. Press 'Calculate' to run the macro that generates the flux data. An average value will be calculated and the graphs will automatically update.

    Note: For this setup, it is expected that for the pure DI water test, a single beaker is used to collect the permeate, as no conductivity measurement is required. More specifically, the scale should be tared with the empty beaker before starting the experiment and collecting mass data.

For NaCl in DI water:

1. Either collect the data directly into the excel file in the 'Mass' column or a text file and copy and paste after the experiment is complete.
2. Add in the conductivity measurements next to the corresponding time.
3. Check that the feed solution concentration, conductivity, effective filtration area for the dead-end cell, and pressure are correct for the given experiment.
4. Check that the mass of the two beakers used to collect the permeate matched the file and add any relevant notes.
4. Adjust the 'Time' column so that each entry in the 'Mass' column has a corresponding time value. Make sure that the 'Time' column does not have any extra values where there is not a matching mass value or the macro will throw an error.
5. Press 'Calculate' to run the macro that generates the flux and rejection data. An average values will be calculated and the graphs will automatically update.

    Note: For this scenario, it expected that two beakers are used to collect solution, and swapped once a sufficent volume of permeate is collected to completely submerge the electrodes of the probe for an accurate conductivity measurement. For this run, the scale is zeroed without the beakers on it so they can be swapped during the experiment.