#Step 1:
Open the pdf file in gimp, use 300 px/in (standard high quality print settings) or high enough 
resolution to ensure the parts will be slightly scaled down, not up (for optimal resolution)

#Step 2:
Do some calculations and scale the image (image->scale image).  See the excel spreadsheet.

#Step 3:
Make a new file with dimensions of the printing paper (8.5x11in in this case).  Make sure the resolution is at least 
300px/in.  Copy the area around the part to be printed from the first, scaled image, and paste into the new file.
Add a text box for a label.  Note GIMP has a bug when saving to PDF--the text scales down considerably, so make sure 
to make text much bigger than it needs to be.  Use the 'Move Layer To' plugin script (http://registry.gimp.org/node/27806)
to be precise and repeatable.

#Step 4:
Open in Adobe reader and print.  Make sure you choose 'Actual Size' in 'Page Sizing and Handling' options.
Measure the dimensions printed and make sure they match up.

#Step 5:
Profit.