% Dynamic Report Generation with R
% Yihui Xie

We import a dataset into a statistical software package, run a procedure to get all results, then copy and paste selected pieces in a typesetting program, add a few descriptions and finish a report. This is a common practice of writing statistical reports. There are obvious dangers and disadvantages of this procedure:

1. it is error-prone due to too much manual work;
1. it requires lots of human efforts to do tedious jobs such as copying results between documents;
1. the workflow is barely recordable especially when it involves with GUI (Graphical User Interface) operations, therefore it is difficult to reproduce;
1. a tiny change of the data source in the future will require the author(s) to go through the same procedure again, which can take nearly the same amount of time and efforts;
1. the analysis and writing are mixed together, so attention has to be paid to the synchronization of the two parts;

A dynamic report is a report generated dynamically from computer code. Just like a software package has its source code, a dynamic report also has its source as a mixture of computer code and normal writings. When we compile the source report, the code in it is executed and replaced with the output; we get a final report by mixing the code output with the original writings. Because we only manage source code, we are free of all the possible problems above. For example, we can change a single parameter in the source code, and get a different report on the fly.

This book is written for those who write reports regularly; the reports here can range from student homework or project reports, exams, books to virtually any documents related to data analysis or statistical graphics and computing.

The main tools we introduce in this book are the R language and the **knitr** package, with which this book is written. We will show how to improve our efficiency in writing reports, fine tune every aspect of a report and go from R output to publication quality reports.

