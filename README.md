A very WIP toolkit to plot data from a Gadgetbridge database. For now, it downsamples data from a MI Band 2 to a resolution of 1 day, then plots a large 2D histogram of heartrate per day, and the sum of steps per day below it. Time resolution and plot sequence can, for now, be set by editing the bottom of `gb_database.py`. In the future, it will be configurable. In principle, other devices should work as well, but I have not been able to test it.

Supported devices:

- MI Band
- HPlus
- NO.1 F1
- Pebble

Available datasets (for MI Band 2, your device may vary):

- heartrate
- activity
- intensity
- steps

There is a minimal sanity checking of heartrate and intensity data. In the future, more extensive filtering will be applied to datasets.

Dependencies:

- Numpy
- matplotlib

Usage (for now): `python gadgetbridge.py databasefile outputfile`