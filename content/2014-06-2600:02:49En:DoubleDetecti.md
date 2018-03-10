En:DoubleDetection
==================

Date: 2014-06-26 00:02:49

[Detect Double Documents Based on Fuzzy Content Signatures:
]{.autocomment}

← Nächstältere Version

Version vom 25. Juni 2014, 22:02 Uhr

Zeile 33:

Zeile 33:

 

<div>

\* create a list of tokens and their quantized frequency, separated by
spaces, in the order of decreasing frequency.

</div>

 

<div>

\* create a list of tokens and their quantized frequency, separated by
spaces, in the order of decreasing frequency.

</div>

 

<div>

The setting for \'\'MIN\_TOKEN\_LEN\'\' and \'\'QUANT\_RATE\'\' can be
done in the servlet at /ContentAnalysis\_p.html. These values influence,
how \'fuzzy\' the attribute works.

</div>

 

<div>

The setting for \'\'MIN\_TOKEN\_LEN\'\' and \'\'QUANT\_RATE\'\' can be
done in the servlet at /ContentAnalysis\_p.html. These values influence,
how \'fuzzy\' the attribute works.

</div>

−

<div>

 After the crawl is finished, a postprocessing counts the number of
documents with the same extact hash and writes the number of such copies
into the field

</div>

\+

<div>

After the crawl is finished, a postprocessing counts the number of
documents with the same extact hash and writes the number of such copies
into the field

</div>

 

<div>

  fuzzy\_signature\_copycount\_i

</div>

 

<div>

  fuzzy\_signature\_copycount\_i

</div>

 

<div>

The flag \'\'fuzzy\_signature\_unique\_b\'\' can be used in the
\[\[En:Ranking\|ranking rules\]\] for filter or boost queries, the
number \'\'fuzzy\_signature\_copycount\_i\'\' can be used for boost
functions.

</div>

 

<div>

The flag \'\'fuzzy\_signature\_unique\_b\'\' can be used in the
\[\[En:Ranking\|ranking rules\]\] for filter or boost queries, the
number \'\'fuzzy\_signature\_copycount\_i\'\' can be used for boost
functions.

</div>
