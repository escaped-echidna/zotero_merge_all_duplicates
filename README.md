# zotero_merge_all_duplicates
Sikuli script which automates merging duplicates in Zotero reference manager software

## Intro
Zotero is really useful for keeping track of citations and building a bibliography. When you import duplicate citations, it helpfully displays all versions of the duplicates in a special folder for you to review and merge. Unfortunately if you have like 5000 sets of duplicates, it is tedious to review all of them and merge them manually. 

Using Sikuli I found a way to automate this process. Sikuli looks at visible elements on the screen and interacts with them using simulated clicks and keyboard actions. I just fire up Zotero and Sikuli, press 'run' on the script, and Sikuli acts just like a human user, clicking 'merge' on each set of duplicates.

## Important notes:

*This will merge duplicates based on whichever version is currently selected by the software to be the default master version. It will not necessarily select the best version of each set of duplicates.*

Also, this was designed for Zotero for Mac - if your UI looks different from mine, you will have to manually change the images that Sikuli uses to find the correct UI elements to click on.

Also also, check the code and modify the values "max_number_of_duplicates" and "pause_between_clicks" to suit your liking.

## Requirements

This script requires that you have a version of 'sikuli' - found here: http://www.sikuli.org/

It is also helpful to have the sikuli IDE and you should have up-to-date Java and Python.
Zotero is also obviously required.
