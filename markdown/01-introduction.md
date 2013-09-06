# Introduction

The big idea is from literate programming, an approach introduced by Donald Knuth. The original idea was mainly for writing software: mix the source code and documentation together; we can either extract the source code out (called _tangle_) or execute the code to get the compiled results (called _weave_). A report is not that different from a computer program: for a report, we need to run software packages to compile our ideas (like source code) into numeric or graphical output, and insert the output into our literal writing (like documentation).

We explain the idea with a trivial example: suppose we need to write the value of $2\pi$ into a report; of course, we can directly write the number $6.28$. Now if I change my mind and I want $6\pi$ instead, I may have to find a calculator, erase the previous value and fill in the new one. Since it is extremely easy for the computer to calculate $6\pi$, why not leave this job to the computer completely and free the man of the labor work? What we need to do is to leave the source code in the document instead of a hard-coded value, and tell the computer how to find out the source code. Usually we use special markups for computer code in the source report, e.g. we can write `'the value is {% 6 * pi %}'`, in which `{%` and `%}` is a pair of marks that tell the computer `6 * pi` is source code and should be executed.

If you know a dynamic web language such as PHP (can mix HTML and PHP code together), the above idea should look familiar. The above example shows the _inline_ code output, which means source code is mixed inline with a sentence. The other type of output is the _chunk_ output, which gives the results from a whole block of code. The chunk output has much more flexibility; for example, we can produce graphics or tables from a code chunk. Here is a plot created with **ggplot2** dynamically:


```r
library(ggplot2)
qplot(hp, mpg, data = mtcars) + geom_smooth()
```

![A sample plot in a dynamic report.](http://i.imgur.com/Vl3qf.png) 


And here is a table created with the **xtable** package:


```r
library(xtable)
xtable(head(mtcars[, 1:5]))
```

<!-- html table generated in R 2.15.1 by xtable 1.7-0 package -->
<!-- Fri Oct 26 14:24:04 2012 -->
<TABLE >
<TR> <TH>  </TH> <TH> mpg </TH> <TH> cyl </TH> <TH> disp </TH> <TH> hp </TH> <TH> drat </TH>  </TR>
  <TR> <TD align="right"> Mazda RX4 </TD> <TD align="right"> 21.00 </TD> <TD align="right"> 6.00 </TD> <TD align="right"> 160.00 </TD> <TD align="right"> 110.00 </TD> <TD align="right"> 3.90 </TD> </TR>
  <TR> <TD align="right"> Mazda RX4 Wag </TD> <TD align="right"> 21.00 </TD> <TD align="right"> 6.00 </TD> <TD align="right"> 160.00 </TD> <TD align="right"> 110.00 </TD> <TD align="right"> 3.90 </TD> </TR>
  <TR> <TD align="right"> Datsun 710 </TD> <TD align="right"> 22.80 </TD> <TD align="right"> 4.00 </TD> <TD align="right"> 108.00 </TD> <TD align="right"> 93.00 </TD> <TD align="right"> 3.85 </TD> </TR>
  <TR> <TD align="right"> Hornet 4 Drive </TD> <TD align="right"> 21.40 </TD> <TD align="right"> 6.00 </TD> <TD align="right"> 258.00 </TD> <TD align="right"> 110.00 </TD> <TD align="right"> 3.08 </TD> </TR>
  <TR> <TD align="right"> Hornet Sportabout </TD> <TD align="right"> 18.70 </TD> <TD align="right"> 8.00 </TD> <TD align="right"> 360.00 </TD> <TD align="right"> 175.00 </TD> <TD align="right"> 3.15 </TD> </TR>
  <TR> <TD align="right"> Valiant </TD> <TD align="right"> 18.10 </TD> <TD align="right"> 6.00 </TD> <TD align="right"> 225.00 </TD> <TD align="right"> 105.00 </TD> <TD align="right"> 2.76 </TD> </TR>
   </TABLE>


TODO: Sweave. An overview of the following chapters.

