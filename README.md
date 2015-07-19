# navigation-spreadsheets
A collection of spreadsheets for performing calculations associated with celestial navigation

The spreadsheets available through this repository are designed to increase the accuracy, reliability,
and the speed with which you can derive your position from  observations of the heavens.  First, you
take a sight with a sextant, make the appropriate corrections to the measured altitude, and retrieve the
necessary astronomical data from an almanac spreadsheet.  Then you enter the data into the appropriate
sight reduction spreadsheet - and you're done!  The use of these spreadsheets finds a middle ground
between manually doing all the steps needed to plot your line of position on a chart and simply pushing
a button to read your location on a GPS receiver.

Our spreadsheets are programmed to provide and process several types of sight data needed in
celestial navigation:

*) Intersections of lines of position 
*) Noon sight and noon curve (including vessel in motion) 
*) Latitude from Polaris 
*) Dead reckoning fix along a line of position
*) Running fix 
*) Sextant altitude corrections 
*) Navigation triangle solutions (the intercept method)
*) Navigation triangle solutions (sailings)
*) Almanac data (Geographical Positions)
*) Lunar distance (UT recovery)

You may use the spreadsheets on any computing platform equipped with an Excel-compatible spreadsheet program
or app (not included in this repository; to be obtained separately from a third-party software provider.
Available choices include Microsoft Excel and OpenOffice Calc.)

A manual describing the use of the spreadsheets is included with the repository.  We assume that you are already
familiar with the principles and terminology of celestial navigation, and the use of sextants and almanacs.
In all spreadsheets the cells expecting the user’s input data are formatted in italics on green background
and the results are displayed with the normal font in cyan cells, all next to labels in bold.  Cells marked
yellow are used for both input and output (i.e. intermediate results). Except in the spreadsheet
aries_stars.xls, the cells containing angular input data are formatted as compound fractions with three-digit
denominators; thus the angle of 27° 31.1´ is to be entered as 27 311/600.  OpenOffice seems to have a problem
here; you may need to reformat these cells using only two-digit fractions and therefore round angles to whole
minutes.  Another alternative is to enter these values using the formula bar as: = 27 + 311/600.  If the value
is negative (e.g. declination S 27° 31.1´), then in the formula you must use minus signs for both the whole
degree component and its fraction: = -27 - 311/600.  Finally, angles (in degrees) can also be entered in
decimal form (27° 31.1´ = 27.5183).

These angular input data are accompanied by grey cells displaying the fractional portion of the data value
in minutes of arc.  This way you can verify that the input value was entered correctly.  You may also use
the minispreadsheet minutes.xls for the same purpose.  Enter the fractional value in cell B1, or the decimal
value in cell B5, and inspect the equivalent angular value in arcminutes.

The formatting of some results does not explicitly separate the sign on output from the integer degree value.
Therefore, for results between -1° and +1° be sure to pick up the correct sign from the decimal value of the
result in a neighboring cell, because zeroes are usually displayed unsigned.

Cells containing time data (with the exception of cell B6 in running_fix.xls, dr.xls, and dr_fix_lop.xls) are
formatted using the 24-hour clock as HH:MM:SS.  (For times between 12 and 1 o’clock make sure that the cell
ends up with the correct AM/PM value.)  All other cell contents represent partial results of the computations
and can be ignored, unless you want to get into the nitty-gritty details.  Our adopted sign convention marks
north latitudes and east longitudes as positive; south latitudes and west longitudes are considered negative;
hour angles increase in the westward direction.  On output, fractions of degrees (minutes of arc) are displayed
without their sign.  We also provide a simple worksheet in which you may record intermediate results, such as
output of almanac spreadsheets that need to be transferred into the input of the sight reduction spreadsheets.
 
For more information you can:
watch a number of demos on: https://www.youtube.com/user/pmh099
visit the blog: https://navigationspreadsheets.wordpress.com/
send inquiries via e-mail to: pmh099@yahoo.com
