# R-utils-and-Scripts
This repo includes various utilities and scripts to analyze microbial genomic data

*stacked_columns.txt*: contains several scripts to obtain a stacked columns graph, useful in representing relative abundances of several metagenomic samples. 
-------------------------------------------------------------------------------------------------------------------------------------------------------------
*Simplify_AssemblyNCBI_Names.txt*: Simplify assembly names downloaded from NCBI
-------------------------------------------------------------------------------
-------------------------------------------------------------
Solution to: Could not load the Qt platform plugin "xcb" #300
-------------------------------------------------------------
 Answered by ben-milanko; ljubomirb asked this question in Q&A

I will leave here solution for a problem that I could not fix for days, hope it would help someone:

So, the error was:

QObject::moveToThread: Current thread (...) is not the object's thread (...).

Cannot move to target thread (...)

qt.qpa.plugin: Could not load the Qt platform plugin "xcb" in "/(...)site-packages/cv2/qt/plugins" even though it was found.

This application failed to start because no Qt platform plugin could be initialized. Reinstalling the application may fix this problem.

In the end, I don't know if that was the fix, because my system is about to be reinstalled after all of my "trying", BUT, after I wrote this in console:

export QT_QPA_PLATFORM=offscreen 
--------------------------------
everything worked.

