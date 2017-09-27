# The Diffusion of the Codex

## Abstract
The adoption of the codex for literature in the Roman world was one of the most significant developments in the history of the book, yet remains poorly understood. Physical evidence seems to contradict literary evidence from Martial’s epigrams. Near-total adoption of the codex for early Christian works, even as the book roll dominated non-Christian book forms in the first centuries of our era, has led to endless speculation about possible ideological motives for adoption. What has been unquestioned is the importance of Christian scribes in the surge of adoption from 300 C.E. onward. This article reexamines the foundation of many theories, the timeline for non-Christian adoption sketched by Roberts and Skeat in their study, <em>The Birth of the Codex,</em> and reevaluates it through the lens of “diffusion of innovations theory” in order to reconcile the evidence and elevate practical considerations once and for all over ideological motives.

(from Classical Antiquity, Vol. 36, Issue 2, pp. 183–235. ISSN: 0278-6656(p); 1067-8344(e)
Copyright © 2017 by The Regents of the University of California.)

## Simulation
As part of research for my article, "The Diffusion of the Codex," I ran Monte Carlo simulations on ancient book finds recorded in the Leuven Database of Ancient Books (LDAB: http://www.trismegistos.org/ldab/index.php) in order to get a clearer picture of the adoption curve for the codex book in the Roman world. For more information consult pp. 211-21 of the article.

## Files
In this repo you will find two tab-separated files. One contains the results of 10,000 simulations on texts from the LDAB matching these characteristics: Greek for the language (or as one of the languages), origin or discovery in Egypt, in codex or roll form, in material parchment or papyrus, and identified as culture: “literature.” Each row has the TM nr for the text, the type (roll or codex), followed by the start and end dates of the date range as determined according to the method on page 47, followed by the midpoint of those dates and the resultant standard deviation if the start and end points had represented 2 standard deviations from the midpoint. These columns are followed by the results of each simulation, first the individual date determined, then the “bucket” that date is placed in. E.g.:

1845 roll −263 −229 −246 8.5 −242 −3 . . .

This file is called simulation_1.tsv.

A second file, simulation_2.tsv, is in the same format but with fewer rows, as it excludes any text which has been tagged with religion: Christian.

There are six additional files: three for each of the simulation runs. A first file has been generated which shows only the frequencies of codices against roll for each of the numbered buckets, which are converted to dates, taking the final year (in fact, the bucket ends on the last day of the previous year) of each bucket for graphing. This is called simulation_n_freq.tsv, where n is the number of the simulation (1 or 2). A second file called simulation_n_avg.tsv (n=1 or 2) contains only the average for the 10,000 simulations. The final file, simulation_n_sc.tsv contains the best-fit S-curve for the respective simulation.

<strong>Note:</strong> simulation_1.tsv and simulation_2.tsv have been stored in this repos as gzipped tarballs due to their size.
