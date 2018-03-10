Dev:SampleServlet.java
======================

Date: 2017-01-01 23:18:49

RequestHeader

← Nächstältere Version

Version vom 1. Januar 2017, 22:18 Uhr

Zeile 1:

Zeile 1:

−

<div>

  import ~~de~~.~~anomic~~.~~server~~.~~\*~~;

</div>

\+

<div>

 

</div>

−

<div>

  import ~~de~~.~~anomic~~.~~plasma~~.~~\*~~;

</div>

\+

<div>

  import
[net]{.underline}.[yacy]{.underline}.[cora]{.underline}.[protocol.RequestHeader]{.underline};

</div>

−

<div>

  import ~~de~~.~~anomic~~.~~http~~.~~\*~~;

</div>

\+

<div>

  import
[net]{.underline}.[yacy]{.underline}.[search]{.underline}.[Switchboard]{.underline};

</div>

 

\+

<div>

  import
[net]{.underline}.[yacy]{.underline}.[server]{.underline}.[serverObjects]{.underline};

</div>

 

\+

<div>

 

</div>

 

<div>

  public class test {

</div>

 

<div>

  public class test {

</div>

−

<div>

     public static serverObjects respond(~~httpHeader~~ header,
serverObjects post, serverSwitch env) {

</div>

\+

<div>

     public static serverObjects respond([RequestHeader]{.underline}
header, serverObjects post, serverSwitch env) {

</div>

−

<div>

     plasmaSwitchboard switchboard = (~~plasmaSwitchboard~~) env;

</div>

\+

<div>

     plasmaSwitchboard switchboard = ([Switchboard]{.underline}) env;

</div>

 

<div>

     serverObjects prop = new serverObjects();

</div>

 

<div>

     serverObjects prop = new serverObjects();

</div>

 

<div>

     if(post != null && post.containsKey(\"num\")){

</div>

 

<div>

     if(post != null && post.containsKey(\"num\")){

</div>
