---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header: no
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
#callforaction:
#  url: https://tinyletter.com/feeling-responsive
#  text: Inform me about new updates and features ›
#  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---


<div class="row">
<div class="large-8 large-push-2 columns" markdown="0">
    
    <h1 id="intel-mpx-explained" style="text-align:center; margin-bottom: 2pt;">Binary Translators for Weak Memory Model Architectures</h1>
    <div style="text-align:center; color: #333;">Tools that correctly translate <em>concurrent</em> x86 binary programs to Armv8</div> 
    <br/>

</div><!-- /.large-6.columns -->
</div><!-- /.row 1 -->

<div class="row">
<div class="medium-12 columns" markdown="1">
----

<h3 style="text-align:center; margin-top: 0; margin-bottom: 1em; font-size: 1.8em;">What is Binary Translation?</h3>

While *x86* previously dominated the CPU market, we see *Arm* emerge prominently in many domains; For instance, on <a href="https://aws.amazon.com/ec2/graviton/" target="_blank">servers</a> and <a href="https://en.wikipedia.org/wiki/Apple_M1" target="_blank">laptops</a>. These architectures have different instruction sets and features, which makes it difficult to port existing x86 programs to Arm CPUs. In particular, these architectures have different *memory models*, which means that x86 and Arm reorder instructions differently during execution. That results in different behavior for the same concurrent programs.

We built *two* binary translators to address this problem, in different ways. *Lasagne* translates any x86 program *statically* to an Arm program. *Risotto* emulates the x86 program *dynamically* on an Arm machine. For either case, we provide *mechanized proofs* that demonstrate the correctness of the translation w.r.t. the memory models of x86 and Arm.

</div>
</div>


<div class="row">
<div class="medium-12 columns" markdown="1">
<!--#### Corresponding publications:-->

<!--* [Our ATC'17 submission "Intel MPX explained"]() _(not yet published)_-->
<!--* [Technical Report "Intel MPX Explained: An Empirical Study of Intel MPX and Software-based Bounds Checking Approaches"](https://arxiv.org/abs/1702.00719)-->
<!--<a href="https://arxiv.org/pdf/1702.00719v1.pdf"><img class="t0" width="3%" src="/images/pdf-icon.png" alt="Technical Report"></a>-->
<!--<a href="/code/tech_rep.bib"><img class="t0" width="3%" src="/images/bibtex.jpg" alt="BibTex"></a>-->
<!--<a href="https://github.com/OleksiiOleksenko/intel_mpx_explained"><img class="t0" width="3%" src="/images/github.png" alt="Source Code"></a>-->

----

<h3 style="text-align:center; margin-top: 0; margin-bottom: 1em; font-size: 1.8em;">Binary Translators</h3>

</div><!-- /.medium-6.columns -->
</div><!-- /.row 2 -->

<div class="row">
<div class="large-6 columns" markdown="0">
    
    <div style="text-align:center;">
        <a href="/lasagne/">
            <img class="t0" width="60%" src="/images/icon_lasagne.webp" alt="Static Binary Translation with Lasagne">
            <h4 style="text-align:center; margin: 0 0 1em 0;">Lasagne<br/>(Static)</h4>
        </a>
    </div>
    
</div><!-- /.large-4.columns -->

<div class="large-6 columns" markdown="0">
    
    <div style="text-align:center;">
        <a href="/risotto/">
            <img class="t0" width="60%" src="/images/icon_risotto.webp" alt="Dynamic Binary Translation with Risotto">
            <h4 style="text-align:center; margin: 0 0 1em 0;">Risotto<br/>(Dynamic)</h4>
        </a>
    </div>
    
</div><!-- /.large-4.columns -->
</div><!-- /.row 3 -->
