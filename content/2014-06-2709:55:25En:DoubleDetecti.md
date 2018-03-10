En:DoubleDetection
==================

Date: 2014-06-27 09:55:25

[Detect Double Documents Based on Fuzzy Content Signatures:
]{.autocomment}

← Nächstältere Version

Version vom 27. Juni 2014, 07:55 Uhr

Zeile 32:

Zeile 32:

 

<div>

\* tokens, which frequency after quantization falls below QUANT, are
discarded.

</div>

 

<div>

\* tokens, which frequency after quantization falls below QUANT, are
discarded.

</div>

 

<div>

\* create a list of tokens and their quantized frequency, separated by
spaces, in the order of decreasing frequency.

</div>

 

<div>

\* create a list of tokens and their quantized frequency, separated by
spaces, in the order of decreasing frequency.

</div>

 

\+

<div>

[\* create a hash of this list. This is the \'fuzzy signature\' which is
compared to the other fuzzy signatures of documents.]{.underline}

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

 

<div>

After the crawl is finished, a postprocessing counts the number of
documents with the same extact hash and writes the number of such copies
into the field

</div>

 

<div>

After the crawl is finished, a postprocessing counts the number of
documents with the same extact hash and writes the number of such copies
into the field

</div>
