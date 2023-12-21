+++
title = 'Audit Analytics'
date = 2023-10-21T15:58:37-05:00
draft = false
+++

![Audit Analytics](/audit_analytics_book_cover.jpg)
[Purchase on Amazon](https://www.amazon.com/Audit-Analytics-Science-Accounting-Profession-ebook/dp/B08NYB2GCQ/ref=sr_1_3?crid=1417UNCLJH3IZ&keywords=audit+analytics&qid=1698079694&sprefix=audit+analytis%2Caps%2C104&sr=8-3)

## The crisis in accounting

Modern auditing was mandated for all publicly listed corporations after the Crash of 1929.  The idea was that the reported book value, suitably audited to validate its truthfulness, would provide an accurate guide to the firm's stock price.   And indeed auditing did provide such assurances, up until the early 1980s.  But since that time, the audited measure of "Book Value" of a firm has steadily diverged from the actual market capitalization of that same firm.  Investors seem to be ignoring the hard work of accountants; indeed they are concluding that auditors and accountants are not really providing useful information for the valuation of a firm.  Look for example at the ratio of book value to market capitalization for the most valuable firms in the US in December 2023:

- Meta/Facebook   17.6%
- Amazon  7.0%
- Apple  2.7%
- Netflix 5.6
- Alphabet/Google 10.1%
- Microsoft 5.3%
- Saudi Aramco  13.2%
- NVIDIA 2.65
- Tesla 0.8%
- Eli Lilly 5.1%

Clearly, most of the value and operations of these cornerstones of the economy are not being reported.   


## How this book came about

I began my career in 1973 as a staff accountant in the Chicago office of Touche Ross (a predecessor firm
to Deloitte Touche Tohmatsu). Computers were new to accounting in those days. IBM had introduced its
System 360 in 1964 (S/360 referred to the architecture's wide scope: 360 degrees to cover the entire circle
of possible uses). By 1973, these were becoming fixtures in the accounting systems of large corporations.
Prior to Touche Ross, I had earned a large portion of my college expenses providing assistance in use of
the Compustat tapes (they were actually physical 9-track tapes in those days, and also came as decks of
80-column Hollerith punched cards) on a Control Data 6600. Touche Ross decided I was well-suited to teach
and develop applications for their bespoke auditing software -- STRATA (System by Touche Ross for Audit
Technical Assistance) and this is largely what I did during the rest of my tenure at Touche Ross.
My Compustat work provided me a prescient foundation in statistical computing which I would later apply
to my auditing work. In those days, people were still calling computers 'electronic brains' reminiscent of
today's use of 'artificial intelligence' to refer to machine learning. Applications of statistical computing to
accounting were poorly taught, and reading matter on the subject was non-existent.


The Compustat story is itself worth retelling, as it played an important role in my education, and has
strong ties to Chicago. Compustat was the brainchild of Alfred Cowles III who came from an established
publishing family; his father and uncle founded the Chicago Tribune and Cleveland Leader, respectively.
For a short time after the first World War, Cowles successfully ran a Chicago investment firm that acquired
and restructured small railroads. His firm also published a stock market newsletter providing fundamental
analysis and recommendations on railroad stock issues as well as other investments. This was long before the
Securities and Exchange Commission existed, let alone required annual audits and reliable financial reports.
Ford Motor company at the time, for example, only produced a balance sheet (unaudited) but not an income
statement, despite being one of the largest firms in the US. It was di?icult to be a financial analyst in those
days.



Diagnosed with tuberculosis in the late 1920s, Cowles consolidated his investments (just prior to the 1929
crash) and moved to Colorado Springs to improve his health. There, he filled his time developing linear re-
gression models that simultaneously compared the predictions of 24 stock market newsletters to actual stock
performance. Cowles quickly came to the conclusion that forecasters were guessing; that they offered little
useful investment information, and were more often wrong than right (he also applied his regression skills
to investigate whether good climates, like Colorado Springs, improved the outcome of tuberculosis, with
somewhat more optimistic results). The pen and paper calculation required at the time, for the regression
formulas he used, soon exceeded his capabilities as a lone researcher. At this point he made a decision to
invest some of his fortune to create the Cowles Commission, an institution dedicated to linking economic
theory to mathematics and statistics. To that end, its mission was to develop a specific, probabilistic frame-
work for estimating simultaneous regression equations to model the U.S. economy. The Cowles Commission
moved from Colorado Springs to the University of Chicago in 1939, where economist Tjalling Koopmans de-
veloped the systems of regression tools that Cowles originally had sought. This period also expanded Cowles
personal files into what ultimately became the Compustat and CRSP databases, and created the market
index that eventually became the Standard & Poor's 500 Index. Cowles researchers developed many new
statistical methods such as the indirect least squares, instrumental variable methods, full information maxi-
mum likelihood method, and limited information maximum likelihood. Eleven Cowles associates ultimately
received the Nobel Prize in Economics.


The days of bespoke auditing software have passed; platforms, systems and standards are too varied and
change too quickly for this small market to be attractive to developers. The good news is that readily available
open-source software now has much more power, flexibility and ease-of-use than has ever been available, and
1these can be applied in the support of audit tasks. Circa 2020, Python, Java and the R statistical packages
are widely used open-source platforms for data analytics; Tensorflow and PyTorch are open-source packages
for machine learning; and open-source packages such as LibreOffice provide spreadsheet capabilities. There
currently are no comprehensive texts for their application in auditing, a fact which motivated the writing of
this book. This book and its methods have grown out of an Audit Analytics course that I have taught at
the University of Illinois -- Chicago, and previously at the Hong Kong University of Science & Technology. I
have switched software platforms several times over the years, but have settled on R, which has become my
software package of choice for data analytics (I talk about motivations for my choice later in this book).
I am honored to be able to contribute my ideas and work in Gentleman, Hornik, and Parmigiani's Use R!
series. Robert Gentleman and Ross Ihaka developed the R programming language at The University of
Auckland in the mid 1990s. Hadley Wickham, who holds adjunct professorships at University of Auckland,
Rice University and Stanford University, has played a major role in developing the tidyverse packages,
which I use throughout this book; and J.J. Allaire's RStudio has put the tools of data analytics within easy
reach of nearly everyone. Researchers such as myself, who regularly confront large, sparse, poorly formatted
business datasets, owe all of them multiple debts of gratitude for not only making our lives infinitely easier,
but also for making some of our research even possible at all.
The Use R! series is designed to make statistical computing tools and relevant algorithms readily available
to practitioners. Since these books are written in LaTeX and R's Bookdown, code for figures and tables
are easily placed on a website for sharing. I assumed, in writing this book, that the reader has a basic
background in statistics (for example, as would be offered in Dalgaard's Introductory Statistics with R) and
in data analytics (for example, as would be offered in Grolemund and Wickham's R for Data Science) and
with basic principles of accounting (for example, as would be offered in Walther's Principals of Accounting).
For the most part, I focus on the tasks faced by an auditor in public accounting, though offer some material
that addresses other important topics in auditing.

## How I intend this Book to be Used

The R language is not a typical language with a single core of developers and guidelines; rather it is a
sharing platform for a wide range of state-of-the-art data analytic functions -- features which make it useful,
dynamic, and sometimes messy. The effort put into familiarizing oneself with the R ecosystem will pay off
many times over in access to the latest, most sophisticated algorithms that exist anywhere in industry.
The reader is assumed to have a basic knowledge of the R language, to be familiar with help screens, with
online package support and documentation sites, and to be linked in with the large group of R experts at
Internet resources like Stack Overflow and R-bloggers. These will be essential resources as the reader
customizes the code examples offered in this text to their own particular needs. Much of the code in this
text, particularly that presented in the Analytical Review chapter, depends on an ever changing set of
databases, streams and standards. In some cases, packages will need to be loaded from GitHub rather than
the o?icial Comprehensive R Archive Network (CRAN) repositories; it is important that the reader consult
these resources as well as CRAN.
In writing this book, I hope to provide the reader with an inventory of basic algorithms which can be easily
expanded and customized to fit an auditor's specific challenges. Accessible and comprehensive tools for
these additional approaches are covered in this book, as are research approaches to take advantage of the
additional explanatory power that these approaches offer to auditing. Coverage of software, methodologies
and fit statistics provide a concise reference for the conduct of audits, helping assure that audit opinions and
decisions are defensible, fair and accurate.

