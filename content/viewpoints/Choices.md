+++
title = 'Auditing & Accounting'
date = 2023-10-21T20:28:09-05:00
draft = false
+++


I began my career in 1973 as a staff accountant in the Chicago office of Touche Ross (a predecessor firm to Deloitte Touche
Tohmatsu). Computers were new to accounting in those days. IBM had introduced its System 360 in 1964 (S/360 referred to
the architecture’s wide scope: 360 degrees to cover the entire circle of possible uses). By 1973, these were becoming fixtures
in the accounting systems of large corporations. 

Prior to Touche Ross, I had earned a large portion of my college expenses
providing assistance in the use of the Compustat tapes (they were actually physical 9-track tapes in those days and also
came as decks of 80-column Hollerith punched cards) on a Control Data 6600. Touche Ross decided I was well-suited to
teach and develop applications for their bespoke auditing software—STRATA (System by Touche Ross for Audit Technical
Assistance) and this is largely what I did during the rest of my tenure at Touche Ross.


My Compustat work provided me a prescient foundation in statistical computing which I would later apply to my
auditing work. In those days, people were still calling computers “electronic brains” reminiscent of today’s use of “artificial
intelligence” to refer to machine learning. Applications of statistical computing to accounting were poorly taught, and reading
matter on the subject was non-existent.


The Compustat story is itself worth retelling, as it played an important role in my education and has strong ties to
Chicago. Compustat was the brainchild of Alfred Cowles III who came from an established publishing family; his father
and uncle founded the Chicago Tribune and Cleveland Leader, respectively. For a short time after the First World War,
Cowles successfully ran a Chicago investment firm that acquired and restructured small railroads. His firm also published
a stock market newsletter providing fundamental analysis and recommendations on railroad stock issues as well as other
investments. This was long before the Securities and Exchange Commission existed, let alone required annual audits and
reliable financial reports. Ford Motor Company at the time, for example, only produced a balance sheet (unaudited) but not
an income statement, despite being one of the largest firms in the USA. It was difficult to be a financial analyst in those days.
Diagnosed with tuberculosis in the late 1920s, Cowles consolidated his investments (just prior to the 1929 crash) and
moved to Colorado Springs to improve his health. There, he filled his time developing linear regression models that
simultaneously compared the predictions of 24 stock market newsletters to actual stock performance. 

Cowles quickly came to the conclusion that forecasters were guessing; that they offered little useful investment information and were more often
wrong than right (he also applied his regression skills to investigate whether good climates, like Colorado Springs, improved
the outcome of tuberculosis, with somewhat more optimistic results). The pen and paper calculation required at the time, for
the regression formulas he used, soon exceeded his capabilities as a lone researcher. At this point, he made a decision to invest
some of his fortune to create the Cowles Commission, an institution dedicated to linking economic theory to mathematics and
statistics. To that end, its mission was to develop a specific, probabilistic framework for estimating simultaneous regression
equations to model the U.S. economy. The Cowles Commission moved from Colorado Springs to the University of Chicago
in 1939, where economist Tjalling Koopmans developed the systems of regression tools that Cowles originally had sought.
This period also expanded Cowles personal files into what ultimately became the Compustat and CRSP databases and created
the market index that eventually became the Standard & Poor’s 500 Index. Cowles researchers developed many new statistical
methods such as the indirect least squares, instrumental variable methods, full information maximum likelihood method, and
limited information maximum likelihood. Eleven Cowles associates ultimately received the Nobel Prize in Economics.


The days of bespoke auditing software have passed; platforms, systems and standards are too varied and change too quickly for this small market to be attractive to developers. The good news is that readily available open-source software now has much more power, flexibility and ease-of-use than has ever been available, and 1these can be applied in the support of audit tasks. Circa 2020, Python, Java and the R statistical packages are widely used open-source platforms for data analytics; Tensorflow and PyTorch are open-source packages for machine learning; and open-source packages such as LibreOffice provide spreadsheet capabilities. There currently are no comprehensive texts for their application in auditing, a fact which motivated the writing of this book. 


My continuing interest in bringing Auditing into the 21st century motivated me to write _"Audit Analytics: Data Science for the Auditing Profession"_. This book and its methods grew out of an Audit Analytics course that I have taught at the University of Illinois – Chicago, and previously at the Hong Kong University of Science & Technology. I have switched software platforms several times over the years, but have settled on R, which has become my software package of choice for data analytics (I talk about motivations for my choice later in this book). 

I was honored, through the publication of _Audit Analytics_, to be able to contribute my ideas and work in Gentleman, Hornik, and Parmigiani’s Use R! series. Robert Gentleman and Ross Ihaka developed the R programming language at The University of Auckland in the mid 1990s. Hadley Wickham, who holds adjunct professorships at University of Auckland, Rice University and Stanford University, has played a major role in developing the tidyverse packages, which I use throughout this book; and J.J. Allaire’s RStudio has put the tools of data analytics within easy reach of nearly everyone. Researchers such as myself, who regularly confront large, sparse, poorly formatted business datasets, owe all of them multiple debts of gratitude for not only making our lives infinitely easier, but also for making some of our research even possible at all. The Use R! series is designed to make statistical computing tools and relevant algorithms readily available to practitioners. Since these books are written in LaTeX and R’s Bookdown, code for figures and tables are easily placed on a website for sharing. I assumed, in writing this book, that the reader has a basic background in statistics (for example, as would be offered in Dalgaard’s Introductory Statistics with R) and in data analytics (for example, as would be offered in Grolemund and Wickham’s R for Data Science) and with basic principles of accounting (for example, as would be offered in Walther’s Principals of Accounting). For the most part, I focus on the tasks faced by an auditor in public accounting, though offer some material that addresses other important topics in auditing.



