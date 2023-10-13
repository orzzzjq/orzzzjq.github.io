---
layout: html
title: Test
date: 2023-10-13 19:07:34
tags:
---

<link href="/blog/ar5iv.min.css" rel="stylesheet"></link>

This post is for testing latexml html file.

<!-- more -->

something more

<!--
<div class="ltx_page_main">
<div class="ltx_page_content">
<article class="ltx_document ltx_authors_1line">
<h1 class="ltx_title ltx_title_document">SVM and Polytope Distance</h1>
<div class="ltx_dates">(October 2023)</div>
<div id="p2" class="ltx_para ltx_noindent">
<p class="ltx_p">Test citation <cite class="ltx_cite ltx_citemacro_cite">[<a href="#bib.bib2" title="Duality and geometry in svm classifiers" class="ltx_ref">1</a>]</cite>.</p>
</div>
<section id="S1" class="ltx_section">
<h2 class="ltx_title ltx_font_bold ltx_title_section" style="font-size:120%;"> Hard-margin SVM</h2>

<div id="S1.p1" class="ltx_para ltx_noindent">
<p class="ltx_p">Given two point sets <math id="S1.p1.m1" class="ltx_Math" alttext="P=\{\bm{u}_{1},\dots,\bm{u}_{n_{1}}\}" display="inline"><mrow><mi>P</mi><mo>=</mo><mrow><mo stretchy="false">{</mo><msub><mi>𝒖</mi><mn>1</mn></msub><mo>,</mo><mi mathvariant="normal">…</mi><mo>,</mo><msub><mi>𝒖</mi><msub><mi>n</mi><mn>1</mn></msub></msub><mo stretchy="false">}</mo></mrow></mrow></math> and <math id="S1.p1.m2" class="ltx_Math" alttext="Q=\{\bm{v}_{1},\dots,\bm{v}_{n_{2}}\}" display="inline"><mrow><mi>Q</mi><mo>=</mo><mrow><mo stretchy="false">{</mo><msub><mi>𝒗</mi><mn>1</mn></msub><mo>,</mo><mi mathvariant="normal">…</mi><mo>,</mo><msub><mi>𝒗</mi><msub><mi>n</mi><mn>2</mn></msub></msub><mo stretchy="false">}</mo></mrow></mrow></math> in <math id="S1.p1.m3" class="ltx_Math" alttext="\bm{R}^{d}" display="inline"><msup><mi>𝑹</mi><mi>d</mi></msup></math>, the polytope distance problem is to find <math id="S1.p1.m4" class="ltx_Math" alttext="\bm{u}\in CH(P),\bm{v}\in CH(Q)" display="inline"><mrow><mrow><mi>𝒖</mi><mo>∈</mo><mrow><mi>C</mi><mo>⁢</mo><mi>H</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>P</mi><mo stretchy="false">)</mo></mrow></mrow></mrow><mo>,</mo><mrow><mi>𝒗</mi><mo>∈</mo><mrow><mi>C</mi><mo>⁢</mo><mi>H</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>Q</mi><mo stretchy="false">)</mo></mrow></mrow></mrow></mrow></math> such that <math id="S1.p1.m5" class="ltx_Math" alttext="\|\bm{u}-\bm{v}\|" display="inline"><mrow><mo>∥</mo><mrow><mi>𝒖</mi><mo>-</mo><mi>𝒗</mi></mrow><mo>∥</mo></mrow></math> is minimized, where <math id="S1.p1.m6" class="ltx_Math" alttext="CH(\cdot)" display="inline"><mrow><mi>C</mi><mo>⁢</mo><mi>H</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mo>⋅</mo><mo stretchy="false">)</mo></mrow></mrow></math> is the convex hull. The problem can be formatted as an optimization problem:</p>
<table id="S1.E1" class="ltx_equationgroup ltx_eqn_table">

<tr id="S1.E1X" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.E1X.m2" class="ltx_Math" alttext="\displaystyle\min_{\bm{\mu},\bm{\lambda}}\quad" display="inline"><mrow><munder><mi>min</mi><mrow><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi></mrow></munder><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E1X.m3" class="ltx_Math" alttext="\displaystyle\frac{1}{2}\|\bm{P\mu}-\bm{Q\lambda}\|^{2}" display="inline"><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>∥</mo></mrow><mn>2</mn></msup></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
<td rowspan="2" class="ltx_eqn_cell ltx_eqn_eqno ltx_align_middle ltx_align_right"><span class="ltx_tag ltx_tag_equationgroup ltx_align_right">(1)</span></td>
</tr>
<tr id="S1.E1Xa" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E1Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{1}^{T}\bm{\mu}=1\quad\bm{1}^{T}\bm{\lambda}=1\quad\bm{\mu},%
\bm{\lambda}\geq 0," display="inline"><mrow><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝁</mi></mrow><mo>=</mo><mn>1</mn></mrow><mo mathvariant="italic" separator="true"> </mo><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝀</mi></mrow><mo>=</mo><mrow><mn>1</mn><mo mathvariant="italic" separator="true"> </mo><mi>𝝁</mi></mrow></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></mrow><mo>,</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
<p class="ltx_p">where <math id="S1.p1.m7" class="ltx_Math" alttext="\bm{P}=(\bm{u}_{1},\dots,\bm{u}_{n_{1}})" display="inline"><mrow><mi>𝑷</mi><mo>=</mo><mrow><mo stretchy="false">(</mo><msub><mi>𝒖</mi><mn>1</mn></msub><mo>,</mo><mi mathvariant="normal">…</mi><mo>,</mo><msub><mi>𝒖</mi><msub><mi>n</mi><mn>1</mn></msub></msub><mo stretchy="false">)</mo></mrow></mrow></math> and <math id="S1.p1.m8" class="ltx_Math" alttext="\bm{Q}=(\bm{v}_{1},\dots,\bm{v}_{n_{2}})" display="inline"><mrow><mi>𝑸</mi><mo>=</mo><mrow><mo stretchy="false">(</mo><msub><mi>𝒗</mi><mn>1</mn></msub><mo>,</mo><mi mathvariant="normal">…</mi><mo>,</mo><msub><mi>𝒗</mi><msub><mi>n</mi><mn>2</mn></msub></msub><mo stretchy="false">)</mo></mrow></mrow></math>.</p>
</div>
<div id="S1.p2" class="ltx_para ltx_noindent">
<p class="ltx_p">Suppose <math id="S1.p2.m1" class="ltx_Math" alttext="P" display="inline"><mi>P</mi></math> and <math id="S1.p2.m2" class="ltx_Math" alttext="Q" display="inline"><mi>Q</mi></math> are linearly separable, i.e. there exists a hyperplane that separates the two points sets, then there exists <math id="S1.p2.m3" class="ltx_Math" alttext="\bm{w}\in\bm{R}^{d}" display="inline"><mrow><mi>𝒘</mi><mo>∈</mo><msup><mi>𝑹</mi><mi>d</mi></msup></mrow></math> and <math id="S1.p2.m4" class="ltx_Math" alttext="\alpha,\beta\in\bm{R}" display="inline"><mrow><mrow><mi>α</mi><mo>,</mo><mi>β</mi></mrow><mo>∈</mo><mi>𝑹</mi></mrow></math>, such that <math id="S1.p2.m5" class="ltx_Math" alttext="\bm{w}^{T}\bm{u}_{i}\geq\alpha\forall\bm{u}_{i}\in P" display="inline"><mrow><mrow><msup><mi>𝒘</mi><mi>T</mi></msup><mo>⁢</mo><msub><mi>𝒖</mi><mi>i</mi></msub></mrow><mo>≥</mo><mrow><mi>α</mi><mo>⁢</mo><mrow><mo>∀</mo><msub><mi>𝒖</mi><mi>i</mi></msub></mrow></mrow><mo>∈</mo><mi>P</mi></mrow></math> and <math id="S1.p2.m6" class="ltx_Math" alttext="\bm{w}^{T}\bm{v}_{i}\leq\beta\forall\bm{v}_{i}\in Q" display="inline"><mrow><mrow><msup><mi>𝒘</mi><mi>T</mi></msup><mo>⁢</mo><msub><mi>𝒗</mi><mi>i</mi></msub></mrow><mo>≤</mo><mrow><mi>β</mi><mo>⁢</mo><mrow><mo>∀</mo><msub><mi>𝒗</mi><mi>i</mi></msub></mrow></mrow><mo>∈</mo><mi>Q</mi></mrow></math>. This is known as the standard support vector machine (SVM). The distance between the two supporting hyperplanes is <math id="S1.p2.m7" class="ltx_Math" alttext="\frac{\alpha-\beta}{\|\bm{w}\|}" display="inline"><mfrac><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow></mfrac></math>. Therefore, the distance between the two planes can be maximized by minimizing <math id="S1.p2.m8" class="ltx_Math" alttext="\|\bm{w}\|" display="inline"><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow></math> and maximizing <math id="S1.p2.m9" class="ltx_Math" alttext="(\alpha-\beta)" display="inline"><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow></math>. This can be written as an optimization problem:</p>
<table id="S1.E2" class="ltx_equationgroup ltx_eqn_table">

<tr id="S1.E2X" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.E2X.m2" class="ltx_Math" alttext="\displaystyle\min_{\bm{w},\alpha,\beta}\quad" display="inline"><mrow><munder><mi>min</mi><mrow><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi></mrow></munder><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E2X.m3" class="ltx_Math" alttext="\displaystyle\frac{1}{2}\|\bm{w}\|^{2}-(\alpha-\beta)" display="inline"><mrow><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
<td rowspan="3" class="ltx_eqn_cell ltx_eqn_eqno ltx_align_middle ltx_align_right"><span class="ltx_tag ltx_tag_equationgroup ltx_align_right">(2)</span></td>
</tr>
<tr id="S1.E2Xa" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E2Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{P}^{T}\bm{w}\geq\alpha\bm{1}" display="inline"><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>≥</mo><mrow><mi>α</mi><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
<tr id="S1.E2Xb" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_eqn_cell"></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E2Xb.m2" class="ltx_Math" alttext="\displaystyle\bm{Q}^{T}\bm{w}\leq\beta\bm{1}." display="inline"><mrow><mrow><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>≤</mo><mrow><mi>β</mi><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
</div>
<div id="Thmclaim1" class="ltx_theorem ltx_theorem_thm">
<h6 class="ltx_title ltx_runin ltx_title_theorem">
<span class="ltx_tag ltx_tag_theorem"><span class="ltx_text ltx_font_bold">Theorem 1</span></span><span class="ltx_text ltx_font_bold">.</span>
</h6>
<div id="Thmclaim1.p1" class="ltx_para">
<p class="ltx_p"><span class="ltx_text ltx_font_italic">Problem (<a href="#S1.E1" title="(1) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">1</span></a>) and Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) are dual of each other.</span></p>
</div>
</div>
<div class="ltx_proof">
<h6 class="ltx_title ltx_runin ltx_font_italic ltx_title_proof">Proof.</h6>
<div id="S1.p3" class="ltx_para">
<p class="ltx_p">The Lagrangian of Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) is:</p>
<table id="S1.Ex1" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex1.m1" class="ltx_Math" alttext="L(\bm{w},\alpha,\beta,\bm{\mu},\bm{\lambda})=\frac{1}{2}\|\bm{w}\|^{2}-(\alpha%
-\beta)-\bm{\mu}^{T}(\bm{P}^{T}\bm{w}-\alpha\bm{1})-\bm{\lambda}^{T}(\beta\bm{%
1}-\bm{Q}^{T}\bm{w})." display="block"><mrow><mrow><mrow><mi>L</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi><mo>,</mo><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mrow><mrow><mfrac><mn>1</mn><mn>2</mn></mfrac><mo>⁢</mo><msup><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow><mo>-</mo><mrow><msup><mi>𝝁</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>-</mo><mrow><mi>α</mi><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>-</mo><mrow><msup><mi>𝝀</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>β</mi><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
<p class="ltx_p">The problem is equivalent to:</p>
<table id="S1.Ex2" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex2.m1" class="ltx_Math" alttext="\min_{\bm{w},\alpha,\beta}\left(\max_{\bm{\mu}\geq 0,\bm{\lambda}\geq 0}L(\bm{%
w},\alpha,\beta,\bm{\mu},\bm{\lambda})\right)." display="block"><mrow><mrow><munder><mi>min</mi><mrow><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi></mrow></munder><mo>⁡</mo><mrow><mo>(</mo><mrow><mrow><munder><mi>max</mi><mrow><mrow><mi>𝝁</mi><mo>≥</mo><mn>0</mn></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></munder><mo>⁡</mo><mi>L</mi></mrow><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi><mo>,</mo><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi><mo stretchy="false">)</mo></mrow></mrow><mo>)</mo></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
<p class="ltx_p">By the minimax theorem, the dual problem is:</p>
<table id="S1.Ex3" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex3.m1" class="ltx_Math" alttext="\max_{\bm{\mu}\geq 0,\bm{\lambda}\geq 0}\left(\min_{\bm{w},\alpha,\beta}L(\bm{%
w},\alpha,\beta,\bm{\mu},\bm{\lambda})\right)." display="block"><mrow><mrow><munder><mi>max</mi><mrow><mrow><mi>𝝁</mi><mo>≥</mo><mn>0</mn></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></munder><mo>⁡</mo><mrow><mo>(</mo><mrow><mrow><munder><mi>min</mi><mrow><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi></mrow></munder><mo>⁡</mo><mi>L</mi></mrow><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi><mo>,</mo><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi><mo stretchy="false">)</mo></mrow></mrow><mo>)</mo></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
<p class="ltx_p">Set <math id="S1.p3.m1" class="ltx_Math" alttext="\frac{\partial L}{\partial\bm{w}}=0,\frac{\partial L}{\partial\alpha}=0,\frac{%
\partial L}{\partial\beta}=0" display="inline"><mrow><mrow><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>𝒘</mi></mrow></mfrac><mo>=</mo><mn>0</mn></mrow><mo>,</mo><mrow><mrow><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>α</mi></mrow></mfrac><mo>=</mo><mn>0</mn></mrow><mo>,</mo><mrow><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>β</mi></mrow></mfrac><mo>=</mo><mn>0</mn></mrow></mrow></mrow></math>, we have:</p>
<table id="S1.Ex4" class="ltx_equationgroup ltx_eqn_table">

<tbody id="S1.Ex4X"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex4X.m2" class="ltx_Math" alttext="\displaystyle\frac{\partial L}{\partial\bm{w}}" display="inline"><mstyle displaystyle="true"><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>𝒘</mi></mrow></mfrac></mstyle></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex4X.m3" class="ltx_Math" alttext="\displaystyle=\bm{w}-\bm{P}\bm{\mu}+\bm{Q}\bm{\lambda}=0" display="inline"><mrow><mi></mi><mo>=</mo><mrow><mrow><mi>𝒘</mi><mo>-</mo><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow></mrow><mo>+</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>=</mo><mn>0</mn></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
<tbody id="S1.Ex4Xa"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex4Xa.m2" class="ltx_Math" alttext="\displaystyle\frac{\partial L}{\partial\alpha}" display="inline"><mstyle displaystyle="true"><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>α</mi></mrow></mfrac></mstyle></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex4Xa.m3" class="ltx_Math" alttext="\displaystyle=-1+\bm{1}^{T}\bm{\mu}=0" display="inline"><mrow><mi></mi><mo>=</mo><mrow><mrow><mo>-</mo><mn>1</mn></mrow><mo>+</mo><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝁</mi></mrow></mrow><mo>=</mo><mn>0</mn></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
<tbody id="S1.Ex4Xb"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex4Xb.m2" class="ltx_Math" alttext="\displaystyle\frac{\partial L}{\partial\beta}" display="inline"><mstyle displaystyle="true"><mfrac><mrow><mo>∂</mo><mo>⁡</mo><mi>L</mi></mrow><mrow><mo>∂</mo><mo>⁡</mo><mi>β</mi></mrow></mfrac></mstyle></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex4Xb.m3" class="ltx_Math" alttext="\displaystyle=1-\bm{1}^{T}\bm{\lambda}=0." display="inline"><mrow><mrow><mi></mi><mo>=</mo><mrow><mn>1</mn><mo>-</mo><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>=</mo><mn>0</mn></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
</table>
<p class="ltx_p">Substitute <math id="S1.p3.m2" class="ltx_Math" alttext="\bm{w}=\bm{P\mu}-\bm{Q\lambda}" display="inline"><mrow><mi>𝒘</mi><mo>=</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow></mrow></math>, the problem becomes:</p>
<table id="S1.Ex5" class="ltx_equationgroup ltx_eqn_table">

<tbody id="S1.Ex5X"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex5X.m2" class="ltx_Math" alttext="\displaystyle\max\quad" display="inline"><mrow><mi>max</mi><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex5X.m3" class="ltx_Math" alttext="\displaystyle\frac{1}{2}\|\bm{P\mu}-\bm{Q\lambda}\|^{2}-(\alpha-\beta)-\bm{\mu%
}^{T}(\bm{P}^{T}(\bm{P\mu}-\bm{Q\lambda})-\alpha\bm{1})-\bm{\lambda}^{T}(\beta%
\bm{1}-\bm{Q}^{T}(\bm{P\mu}-\bm{Q\lambda}))" display="inline"><mrow><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow><mo>-</mo><mrow><msup><mi>𝝁</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>-</mo><mrow><mi>α</mi><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>-</mo><mrow><msup><mi>𝝀</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>β</mi><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
<tbody id="S1.Ex5Xa"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex5Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{1}^{T}\bm{\mu}=1\quad\bm{1}^{T}\bm{\lambda}=1\quad\bm{\mu},%
\bm{\lambda}\geq 0," display="inline"><mrow><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝁</mi></mrow><mo>=</mo><mn>1</mn></mrow><mo mathvariant="italic" separator="true"> </mo><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝀</mi></mrow><mo>=</mo><mrow><mn>1</mn><mo mathvariant="italic" separator="true"> </mo><mi>𝝁</mi></mrow></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></mrow><mo>,</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
</table>
<p class="ltx_p">which simplifies to</p>
<table id="S1.Ex6" class="ltx_equationgroup ltx_eqn_table">

<tbody id="S1.Ex6X"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex6X.m2" class="ltx_Math" alttext="\displaystyle\max\quad" display="inline"><mrow><mi>max</mi><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex6X.m3" class="ltx_Math" alttext="\displaystyle\frac{1}{2}\|\bm{P\mu}-\bm{Q\lambda}\|^{2}-(\alpha-\beta)+\alpha-%
\beta+(\bm{Q\lambda}-\bm{P\mu})^{T}(\bm{P\mu}-\bm{Q\lambda})" display="inline"><mrow><mrow><mrow><mrow><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>+</mo><mi>α</mi></mrow><mo>-</mo><mi>β</mi></mrow><mo>+</mo><mrow><msup><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow><mo>-</mo><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow></mrow><mo stretchy="false">)</mo></mrow><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
<tbody id="S1.Ex6Xa"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex6Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{1}^{T}\bm{\mu}=1\quad\bm{1}^{T}\bm{\lambda}=1\quad\bm{\mu},%
\bm{\lambda}\geq 0," display="inline"><mrow><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝁</mi></mrow><mo>=</mo><mn>1</mn></mrow><mo mathvariant="italic" separator="true"> </mo><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝀</mi></mrow><mo>=</mo><mrow><mn>1</mn><mo mathvariant="italic" separator="true"> </mo><mi>𝝁</mi></mrow></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></mrow><mo>,</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
</table>
<p class="ltx_p">and can be further simplified to</p>
<table id="S1.Ex7" class="ltx_equationgroup ltx_eqn_table">

<tbody id="S1.Ex7X"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex7X.m2" class="ltx_Math" alttext="\displaystyle\max\quad" display="inline"><mrow><mi>max</mi><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex7X.m3" class="ltx_Math" alttext="\displaystyle-\frac{1}{2}\|\bm{P\mu}-\bm{Q\lambda}\|^{2}" display="inline"><mrow><mo>-</mo><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mi>𝝁</mi></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mi>𝝀</mi></mrow></mrow><mo>∥</mo></mrow><mn>2</mn></msup></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
<tbody id="S1.Ex7Xa"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.Ex7Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{1}^{T}\bm{\mu}=1\quad\bm{1}^{T}\bm{\lambda}=1\quad\bm{\mu},%
\bm{\lambda}\geq 0," display="inline"><mrow><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝁</mi></mrow><mo>=</mo><mn>1</mn></mrow><mo mathvariant="italic" separator="true"> </mo><mrow><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mi>𝝀</mi></mrow><mo>=</mo><mrow><mn>1</mn><mo mathvariant="italic" separator="true"> </mo><mi>𝝁</mi></mrow></mrow><mo>,</mo><mrow><mi>𝝀</mi><mo>≥</mo><mn>0</mn></mrow></mrow></mrow><mo>,</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
</table>
<p class="ltx_p">which is equivalent to Problem (<a href="#S1.E1" title="(1) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">1</span></a>) and completes the proof.
∎</p>
</div>
</div>
<div id="S1.p4" class="ltx_para ltx_noindent">
<p class="ltx_p">If we fix <math id="S1.p4.m1" class="ltx_Math" alttext="\alpha-\beta=2" display="inline"><mrow><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo>=</mo><mn>2</mn></mrow></math> by defining <math id="S1.p4.m2" class="ltx_Math" alttext="\alpha=\gamma+1" display="inline"><mrow><mi>α</mi><mo>=</mo><mrow><mi>γ</mi><mo>+</mo><mn>1</mn></mrow></mrow></math> and <math id="S1.p4.m3" class="ltx_Math" alttext="\beta=\gamma-1" display="inline"><mrow><mi>β</mi><mo>=</mo><mrow><mi>γ</mi><mo>-</mo><mn>1</mn></mrow></mrow></math>, Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) becomes:</p>
<table id="S1.E3" class="ltx_equationgroup ltx_eqn_table">

<tr id="S1.E3X" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.E3X.m2" class="ltx_Math" alttext="\displaystyle\min_{\bm{w},\gamma}\quad" display="inline"><mrow><munder><mi>min</mi><mrow><mi>𝒘</mi><mo>,</mo><mi>γ</mi></mrow></munder><mo mathvariant="italic" separator="true"> </mo></mrow></math></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E3X.m3" class="ltx_Math" alttext="\displaystyle\frac{1}{2}\|\bm{w}\|^{2}" display="inline"><mrow><mstyle displaystyle="true"><mfrac><mn>1</mn><mn>2</mn></mfrac></mstyle><mo>⁢</mo><msup><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow><mn>2</mn></msup></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
<td rowspan="3" class="ltx_eqn_cell ltx_eqn_eqno ltx_align_middle ltx_align_right"><span class="ltx_tag ltx_tag_equationgroup ltx_align_right">(3)</span></td>
</tr>
<tr id="S1.E3Xa" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell">
<span class="ltx_text ltx_markedasmath ltx_font_italic">s.t.</span><span class="ltx_text ltx_font_italic"></span>
</td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E3Xa.m3" class="ltx_Math" alttext="\displaystyle\bm{P}^{T}\bm{w}\geq(1+\gamma)\bm{1}" display="inline"><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>≥</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mn>1</mn><mo>+</mo><mi>γ</mi></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
<tr id="S1.E3Xb" class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_eqn_cell"></td>
<td class="ltx_td ltx_align_left ltx_eqn_cell"><math id="S1.E3Xb.m2" class="ltx_Math" alttext="\displaystyle-\bm{Q}^{T}\bm{w}\leq(1-\gamma)\bm{1}." display="inline"><mrow><mrow><mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow></mrow><mo>≤</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mn>1</mn><mo>-</mo><mi>γ</mi></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
</div>
<div id="Thmclaim2" class="ltx_theorem ltx_theorem_thm">
<h6 class="ltx_title ltx_runin ltx_title_theorem">
<span class="ltx_tag ltx_tag_theorem"><span class="ltx_text ltx_font_bold">Theorem 2</span></span><span class="ltx_text ltx_font_bold">.</span>
</h6>
<div id="Thmclaim2.p1" class="ltx_para">
<p class="ltx_p"><span class="ltx_text ltx_font_italic">If <math id="Thmclaim2.p1.m1" class="ltx_Math" alttext="P" display="inline"><mi>P</mi></math> and <math id="Thmclaim2.p1.m2" class="ltx_Math" alttext="Q" display="inline"><mi>Q</mi></math> are linearly separable, i.e. <math id="Thmclaim2.p1.m3" class="ltx_Math" alttext="\frac{1}{2}\|\bm{P\mu}-\bm{Q\lambda}\|^{2}&gt;0" display="inline"><mrow><mrow><mfrac><mn mathvariant="normal">1</mn><mn mathvariant="normal">2</mn></mfrac><mo mathvariant="italic">⁢</mo><msup><mrow><mo mathvariant="normal">∥</mo><mrow><mrow><mi>𝐏</mi><mo mathvariant="italic">⁢</mo><mi>𝛍</mi></mrow><mo mathvariant="normal">-</mo><mrow><mi>𝐐</mi><mo mathvariant="italic">⁢</mo><mi>𝛌</mi></mrow></mrow><mo mathvariant="normal">∥</mo></mrow><mn mathvariant="normal">2</mn></msup></mrow><mo mathvariant="normal">&gt;</mo><mn mathvariant="normal">0</mn></mrow></math>,
Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) and Problem (<a href="#S1.E3" title="(3) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">3</span></a>) are equivalent.</span></p>
</div>
</div>
<div class="ltx_proof">
<h6 class="ltx_title ltx_runin ltx_font_italic ltx_title_proof">Proof.</h6>
<div id="S1.p5" class="ltx_para ltx_noindent">
<p class="ltx_p">Recall the Lagrangian of Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) is:</p>
<table id="S1.Ex8" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex8.m1" class="ltx_Math" alttext="L(\bm{w},\alpha,\beta,\bm{\mu},\bm{\lambda})=\frac{1}{2}\|\bm{w}\|^{2}-(\alpha%
-\beta)-\bm{\mu}^{T}(\bm{P}^{T}\bm{w}-\alpha\bm{1})-\bm{\lambda}^{T}(\beta\bm{%
1}-\bm{Q}^{T}\bm{w})." display="block"><mrow><mrow><mrow><mi>L</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>𝒘</mi><mo>,</mo><mi>α</mi><mo>,</mo><mi>β</mi><mo>,</mo><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mrow><mrow><mfrac><mn>1</mn><mn>2</mn></mfrac><mo>⁢</mo><msup><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><mo stretchy="false">(</mo><mrow><mi>α</mi><mo>-</mo><mi>β</mi></mrow><mo stretchy="false">)</mo></mrow><mo>-</mo><mrow><msup><mi>𝝁</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>-</mo><mrow><mi>α</mi><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>-</mo><mrow><msup><mi>𝝀</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mi>β</mi><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
</div>
<div id="S1.p6" class="ltx_para ltx_noindent">
<p class="ltx_p">Each KKT point <math id="S1.p6.m1" class="ltx_Math" alttext="(\bar{\bm{w}},\bar{\alpha},\bar{\beta},\bar{\bm{\mu}},\bar{\bm{\lambda}})" display="inline"><mrow><mo stretchy="false">(</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover><mo>,</mo><mover accent="true"><mi>α</mi><mo stretchy="false">¯</mo></mover><mo>,</mo><mover accent="true"><mi>β</mi><mo stretchy="false">¯</mo></mover><mo>,</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">¯</mo></mover><mo>,</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">¯</mo></mover><mo stretchy="false">)</mo></mrow></math> of Problem (<a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>) satisfies</p>
<table id="S1.E4" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.E4.m1" class="ltx_Math" alttext="\begin{aligned} \bm{P}\bar{\bm{\mu}}-\bm{Q}\bar{\bm{\lambda}}=\bar{\bm{w}}&amp;\\
\bm{1}^{T}\bar{\bm{\mu}}=1&amp;\\
\bm{1}^{T}\bar{\bm{\lambda}}=1&amp;\end{aligned}\quad\quad\begin{aligned} \bar{\bm%
{\mu}}^{T}(\bm{P}^{T}\bar{\bm{w}}-\bar{\alpha}\bm{1})=0&amp;\\
\bar{\bm{\lambda}}^{T}(\bar{\beta}\bm{1}-\bm{Q}^{T}\bar{\bm{w}})=0&amp;\end{%
aligned}\quad\quad\begin{aligned} \bm{P}^{T}\bar{\bm{w}}\geq\bar{\alpha}\bm{1}%
&amp;\\
\bm{Q}^{T}\bar{\bm{w}}\leq\bar{\beta}\bm{1}&amp;\end{aligned}\quad\quad\begin{%
aligned} \bar{\bm{\mu}}&amp;\geq 0\\
\bar{\bm{\lambda}}&amp;\geq 0\end{aligned}" display="block"><mrow><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">¯</mo></mover></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">¯</mo></mover></mrow></mrow><mo>=</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">¯</mo></mover></mrow><mo>=</mo><mn>1</mn></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">¯</mo></mover></mrow><mo>=</mo><mn>1</mn></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><msup><mover accent="true"><mi>𝝁</mi><mo stretchy="false">¯</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow><mo>-</mo><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">¯</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mn>0</mn></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mover accent="true"><mi>𝝀</mi><mo stretchy="false">¯</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mover accent="true"><mi>β</mi><mo stretchy="false">¯</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mn>0</mn></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow><mo>≥</mo><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">¯</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow><mo>≤</mo><mrow><mover accent="true"><mi>β</mi><mo stretchy="false">¯</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝁</mi><mo stretchy="false">¯</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝀</mi><mo stretchy="false">¯</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr></mtable></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
<td rowspan="1" class="ltx_eqn_cell ltx_eqn_eqno ltx_align_middle ltx_align_right"><span class="ltx_tag ltx_tag_equation ltx_align_right">(4)</span></td>
</tr>
</table>
</div>
<div id="S1.p7" class="ltx_para ltx_noindent">
<p class="ltx_p">The Lagrangian of Problem (<a href="#S1.E3" title="(3) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">3</span></a>) is:</p>
<table id="S1.Ex9" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex9.m1" class="ltx_Math" alttext="L(\bm{w},\gamma,\bm{\mu},\bm{\lambda})=\frac{1}{2}\|\bm{w}\|^{2}-\bm{\mu}^{T}(%
\bm{P}^{T}\bm{w}-(1+\gamma)\bm{1})-\bm{\lambda}^{T}((\gamma-1)-\bm{Q}^{T}\bm{w%
})." display="block"><mrow><mrow><mrow><mi>L</mi><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mi>𝒘</mi><mo>,</mo><mi>γ</mi><mo>,</mo><mi>𝝁</mi><mo>,</mo><mi>𝝀</mi><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mrow><mrow><mfrac><mn>1</mn><mn>2</mn></mfrac><mo>⁢</mo><msup><mrow><mo>∥</mo><mi>𝒘</mi><mo>∥</mo></mrow><mn>2</mn></msup></mrow><mo>-</mo><mrow><msup><mi>𝝁</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow><mo>-</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mn>1</mn><mo>+</mo><mi>γ</mi></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>-</mo><mrow><msup><mi>𝝀</mi><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mi>γ</mi><mo>-</mo><mn>1</mn></mrow><mo stretchy="false">)</mo></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mi>𝒘</mi></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mrow></mrow><mo>.</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
</div>
<div id="S1.p8" class="ltx_para ltx_noindent">
<p class="ltx_p">Each KKT point <math id="S1.p8.m1" class="ltx_Math" alttext="(\hat{\bm{w}},\hat{\gamma},\hat{\bm{\mu}},\hat{\bm{\lambda}})" display="inline"><mrow><mo stretchy="false">(</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">^</mo></mover><mo>,</mo><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover><mo>,</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover><mo>,</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover><mo stretchy="false">)</mo></mrow></math> of Problem (<a href="#S1.E3" title="(3) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">3</span></a>) satisfies:</p>
<table id="S1.E5" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.E5.m1" class="ltx_Math" alttext="\begin{aligned} \bm{P}\hat{\bm{\mu}}-\bm{Q}\hat{\bm{\lambda}}=\hat{\bm{w}}&amp;\\
\bm{1}^{T}\hat{\bm{\mu}}=\bm{1}^{T}\hat{\bm{\lambda}}&amp;\end{aligned}\quad\quad%
\begin{aligned} \hat{\bm{\mu}}^{T}(\bm{P}^{T}\hat{\bm{w}}-(1+\hat{\gamma})\bm{%
1})&amp;=0\\
\hat{\bm{\lambda}}^{T}((\hat{\gamma}-1)\bm{1}-\bm{Q}^{T}\hat{\bm{w}})&amp;=0\end{%
aligned}\quad\quad\begin{aligned} \bm{P}^{T}\bar{\bm{w}}&amp;\geq(1+\hat{\gamma})%
\bm{1}\\
\bm{Q}^{T}\bar{\bm{w}}&amp;\leq(\hat{\gamma}-1)\bm{1}\end{aligned}\quad\quad\begin%
{aligned} \hat{\bm{\mu}}&amp;\geq 0\\
\hat{\bm{\lambda}}&amp;\geq 0\end{aligned}" display="block"><mrow><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover></mrow></mrow><mo>=</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">^</mo></mover></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover></mrow><mo>=</mo><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover></mrow></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><msup><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">^</mo></mover></mrow><mo>-</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mn>1</mn><mo>+</mo><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mtd><mtd columnalign="left"><mrow><mi></mi><mo>=</mo><mn>0</mn></mrow></mtd></mtr><mtr><mtd columnalign="right"><mrow><msup><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mrow><mo stretchy="false">(</mo><mrow><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover><mo>-</mo><mn>1</mn></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">^</mo></mover></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow></mtd><mtd columnalign="left"><mrow><mi></mi><mo>=</mo><mn>0</mn></mrow></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mn>1</mn><mo>+</mo><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd></mtr><mtr><mtd columnalign="right"><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">¯</mo></mover></mrow></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≤</mo><mrow><mrow><mo stretchy="false">(</mo><mrow><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover><mo>-</mo><mn>1</mn></mrow><mo stretchy="false">)</mo></mrow><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" displaystyle="true" rowspacing="0pt"><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr></mtable></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
<td rowspan="1" class="ltx_eqn_cell ltx_eqn_eqno ltx_align_middle ltx_align_right"><span class="ltx_tag ltx_tag_equation ltx_align_right">(5)</span></td>
</tr>
</table>
</div>
<div id="S1.p9" class="ltx_para">
<p class="ltx_p">Assuming <math id="S1.p9.m1" class="ltx_Math" alttext="\tilde{\alpha}-\tilde{\beta}&gt;0" display="inline"><mrow><mrow><mover accent="true"><mi mathcolor="#0000FF">α</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover><mo mathcolor="#0000FF">-</mo><mover accent="true"><mi mathcolor="#0000FF">β</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover></mrow><mo mathcolor="#0000FF">&gt;</mo><mn mathcolor="#0000FF">0</mn></mrow></math>, set <math id="S1.p9.m2" class="ltx_Math" alttext="\delta=\frac{2}{\tilde{\alpha}-\tilde{\beta}}" display="inline"><mrow><mi>δ</mi><mo>=</mo><mfrac><mn>2</mn><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">~</mo></mover><mo>-</mo><mover accent="true"><mi>β</mi><mo stretchy="false">~</mo></mover></mrow></mfrac></mrow></math>, <math id="S1.p9.m3" class="ltx_Math" alttext="\tilde{\alpha}=\frac{\hat{\gamma}+1}{\delta}" display="inline"><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">~</mo></mover><mo>=</mo><mfrac><mrow><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover><mo>+</mo><mn>1</mn></mrow><mi>δ</mi></mfrac></mrow></math>, <math id="S1.p9.m4" class="ltx_Math" alttext="\tilde{\beta}=\frac{\hat{\gamma}-1}{\delta}" display="inline"><mrow><mover accent="true"><mi>β</mi><mo stretchy="false">~</mo></mover><mo>=</mo><mfrac><mrow><mover accent="true"><mi>γ</mi><mo stretchy="false">^</mo></mover><mo>-</mo><mn>1</mn></mrow><mi>δ</mi></mfrac></mrow></math>, <math id="S1.p9.m5" class="ltx_Math" alttext="\tilde{\bm{w}}=\frac{\hat{\bm{w}}}{\delta}" display="inline"><mrow><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover><mo>=</mo><mfrac><mover accent="true"><mi>𝒘</mi><mo stretchy="false">^</mo></mover><mi>δ</mi></mfrac></mrow></math>, <math id="S1.p9.m6" class="ltx_Math" alttext="\tilde{\bm{\mu}}=\frac{\hat{\bm{\mu}}}{\delta}" display="inline"><mrow><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover><mo>=</mo><mfrac><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover><mi>δ</mi></mfrac></mrow></math>, <math id="S1.p9.m7" class="ltx_Math" alttext="\tilde{\bm{\lambda}}=\frac{\hat{\bm{\lambda}}}{\delta}" display="inline"><mrow><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover><mo>=</mo><mfrac><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover><mi>δ</mi></mfrac></mrow></math> and <math id="S1.p9.m8" class="ltx_Math" alttext="\bm{1}^{T}\hat{\bm{\mu}}=\bm{1}^{T}\hat{\bm{\lambda}}=\delta" display="inline"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">^</mo></mover></mrow><mo>=</mo><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">^</mo></mover></mrow><mo>=</mo><mi>δ</mi></mrow></math>, and divide each KKT condition in (<a href="#S1.E5" title="(5) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">5</span></a>) by <math id="S1.p9.m9" class="ltx_Math" alttext="\delta" display="inline"><mi>δ</mi></math> or <math id="S1.p9.m10" class="ltx_Math" alttext="\delta^{2}" display="inline"><msup><mi>δ</mi><mn>2</mn></msup></math>, we have</p>
<table id="S1.Ex10" class="ltx_equationgroup ltx_eqn_table">

<tbody id="S1.Ex10X"><tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_td ltx_align_right ltx_eqn_cell"><math id="S1.Ex10X.m2" class="ltx_Math" alttext="\displaystyle\begin{aligned} \bm{P}\tilde{\bm{\mu}}-\bm{Q}\tilde{\bm{\lambda}}%
=\tilde{\bm{w}}&amp;\\
\bm{1}^{T}\tilde{\bm{\mu}}=1&amp;\\
\bm{1}^{T}\tilde{\bm{\lambda}}=1&amp;\end{aligned}\quad\quad\begin{aligned} \tilde%
{\bm{\mu}}^{T}(\bm{P}^{T}\tilde{\bm{w}}-\tilde{\alpha}\bm{1})=0&amp;\\
\tilde{\bm{\lambda}}^{T}(\tilde{\beta}\bm{1}-\bm{Q}^{T}\tilde{\bm{w}})=0&amp;\end{%
aligned}\quad\quad\begin{aligned} \bm{P}^{T}\tilde{\bm{w}}\geq\tilde{\alpha}%
\bm{1}&amp;\\
\bm{Q}^{T}\tilde{\bm{w}}\leq\tilde{\beta}\bm{1}&amp;\end{aligned}\quad\quad\begin{%
aligned} \tilde{\bm{\mu}}&amp;\geq 0\\
\tilde{\bm{\lambda}}&amp;\geq 0\end{aligned}" display="inline"><mrow><mtable columnspacing="0pt" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><mrow><mi>𝑷</mi><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover></mrow><mo>-</mo><mrow><mi>𝑸</mi><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover></mrow></mrow><mo>=</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover></mrow><mo>=</mo><mn>1</mn></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mn>𝟏</mn><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover></mrow><mo>=</mo><mn>1</mn></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><msup><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover></mrow><mo>-</mo><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">~</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mn>0</mn></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover><mi>T</mi></msup><mo>⁢</mo><mrow><mo stretchy="false">(</mo><mrow><mrow><mover accent="true"><mi>β</mi><mo stretchy="false">~</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow><mo>-</mo><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover></mrow></mrow><mo stretchy="false">)</mo></mrow></mrow><mo>=</mo><mn>0</mn></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" rowspacing="0pt"><mtr><mtd columnalign="right"><mrow><mrow><msup><mi>𝑷</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover></mrow><mo>≥</mo><mrow><mover accent="true"><mi>α</mi><mo stretchy="false">~</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd><mtd></mtd></mtr><mtr><mtd columnalign="right"><mrow><mrow><msup><mi>𝑸</mi><mi>T</mi></msup><mo>⁢</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover></mrow><mo>≤</mo><mrow><mover accent="true"><mi>β</mi><mo stretchy="false">~</mo></mover><mo>⁢</mo><mn>𝟏</mn></mrow></mrow></mtd><mtd></mtd></mtr></mtable><mo mathvariant="italic" separator="true">  </mo><mtable columnspacing="0pt" rowspacing="0pt"><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr><mtr><mtd columnalign="right"><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover></mtd><mtd columnalign="left"><mrow><mi></mi><mo>≥</mo><mn>0</mn></mrow></mtd></mtr></mtable></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr></tbody>
</table>
<p class="ltx_p">which coincides with the KKT condition (<a href="#S1.E4" title="(4) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">4</span></a>) and implies that <math id="S1.p9.m11" class="ltx_Math" alttext="(\tilde{\bm{w}},\tilde{\alpha},\tilde{\beta},\tilde{\bm{\mu}},\tilde{\bm{%
\lambda}})" display="inline"><mrow><mo stretchy="false">(</mo><mover accent="true"><mi>𝒘</mi><mo stretchy="false">~</mo></mover><mo>,</mo><mover accent="true"><mi>α</mi><mo stretchy="false">~</mo></mover><mo>,</mo><mover accent="true"><mi>β</mi><mo stretchy="false">~</mo></mover><mo>,</mo><mover accent="true"><mi>𝝁</mi><mo stretchy="false">~</mo></mover><mo>,</mo><mover accent="true"><mi>𝝀</mi><mo stretchy="false">~</mo></mover><mo stretchy="false">)</mo></mrow></math> is a KKT point to Problem <a href="#S1.E2" title="(2) ‣ Hard-margin SVM ‣ SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_tag">2</span></a>. <span class="ltx_text" style="color:#0000FF;"> Since <math id="S1.p9.m12" class="ltx_Math" alttext="P" display="inline"><mi mathcolor="#0000FF">P</mi></math> and <math id="S1.p9.m13" class="ltx_Math" alttext="Q" display="inline"><mi mathcolor="#0000FF">Q</mi></math> are linearly separable, by strong duality, we have</span></p>
<table id="S1.Ex11" class="ltx_equation ltx_eqn_table">

<tr class="ltx_equation ltx_eqn_row ltx_align_baseline">
<td class="ltx_eqn_cell ltx_eqn_center_padleft"></td>
<td class="ltx_eqn_cell ltx_align_center"><math id="S1.Ex11.m1" class="ltx_Math" alttext="\frac{1}{2}\|\tilde{\bm{w}}\|^{2}-(\tilde{\alpha}-\tilde{\beta})=-\frac{1}{2}%
\|\bm{P}\tilde{\bm{\mu}}-\bm{Q}\tilde{\bm{\lambda}}\|^{2}&lt;0," display="block"><mrow><mrow><mrow><mrow><mfrac mathcolor="#0000FF"><mn mathcolor="#0000FF">1</mn><mn mathcolor="#0000FF">2</mn></mfrac><mo mathcolor="#0000FF">⁢</mo><msup><mrow><mo mathcolor="#0000FF">∥</mo><mover accent="true"><mi mathcolor="#0000FF">𝒘</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover><mo mathcolor="#0000FF">∥</mo></mrow><mn mathcolor="#0000FF">2</mn></msup></mrow><mo mathcolor="#0000FF">-</mo><mrow><mo mathcolor="#0000FF" stretchy="false">(</mo><mrow><mover accent="true"><mi mathcolor="#0000FF">α</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover><mo mathcolor="#0000FF">-</mo><mover accent="true"><mi mathcolor="#0000FF">β</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover></mrow><mo mathcolor="#0000FF" stretchy="false">)</mo></mrow></mrow><mo mathcolor="#0000FF">=</mo><mrow><mo mathcolor="#0000FF">-</mo><mrow><mfrac mathcolor="#0000FF"><mn mathcolor="#0000FF">1</mn><mn mathcolor="#0000FF">2</mn></mfrac><mo mathcolor="#0000FF">⁢</mo><msup><mrow><mo mathcolor="#0000FF">∥</mo><mrow><mrow><mi mathcolor="#0000FF">𝑷</mi><mo mathcolor="#0000FF">⁢</mo><mover accent="true"><mi mathcolor="#0000FF">𝝁</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover></mrow><mo mathcolor="#0000FF">-</mo><mrow><mi mathcolor="#0000FF">𝑸</mi><mo mathcolor="#0000FF">⁢</mo><mover accent="true"><mi mathcolor="#0000FF">𝝀</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover></mrow></mrow><mo mathcolor="#0000FF">∥</mo></mrow><mn mathcolor="#0000FF">2</mn></msup></mrow></mrow><mo mathcolor="#0000FF">&lt;</mo><mn mathcolor="#0000FF">0</mn></mrow><mo mathcolor="#0000FF">,</mo></mrow></math></td>
<td class="ltx_eqn_cell ltx_eqn_center_padright"></td>
</tr>
</table>
<p class="ltx_p"><span class="ltx_text" style="color:#0000FF;">which verifies our assumption <math id="S1.p9.m14" class="ltx_Math" alttext="\tilde{\alpha}-\tilde{\beta}&gt;0" display="inline"><mrow><mrow><mover accent="true"><mi mathcolor="#0000FF">α</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover><mo mathcolor="#0000FF">-</mo><mover accent="true"><mi mathcolor="#0000FF">β</mi><mo mathcolor="#0000FF" stretchy="false">~</mo></mover></mrow><mo mathcolor="#0000FF">&gt;</mo><mn mathcolor="#0000FF">0</mn></mrow></math>.
</span>
∎</p>
</div>
</div>
<div id="S1.p10" class="ltx_para">
<p class="ltx_p"></p>
</div>
</section>
<section id="bib" class="ltx_bibliography">
<h2 class="ltx_title ltx_title_bibliography">References</h2>

<ul id="bib.L1" class="ltx_biblist">
<li id="bib.bib2" class="ltx_bibitem ltx_bib_inproceedings">
<span class="ltx_tag ltx_bib_key ltx_role_refnum ltx_tag_bibitem">[1]</span>
<span class="ltx_bibblock"><span class="ltx_text ltx_bib_author">K. P. Bennett and E. J. Bredensteiner</span><span class="ltx_text ltx_bib_year"> (2000)</span>
</span>
<span class="ltx_bibblock"><span class="ltx_text ltx_bib_title">Duality and geometry in svm classifiers</span>.
</span>
<span class="ltx_bibblock">In <span class="ltx_text ltx_bib_inbook">ICML</span>,
</span>
<span class="ltx_bibblock">Vol. <span class="ltx_text ltx_bib_volume">2000</span>, <span class="ltx_text ltx_bib_pages"> pp. 57–64</span>.
</span>
<span class="ltx_bibblock ltx_bib_cited">Cited by: <a href="#p2" title="SVM and Polytope Distance" class="ltx_ref"><span class="ltx_text ltx_ref_title">SVM and Polytope Distance</span></a>.
</span>
</li>
</ul>
</section>
</article>
</div>
<footer class="ltx_page_footer">
<div class="ltx_page_logo">Generated  on Fri Oct 13 17:52:31 2023 by <a href="http://dlmf.nist.gov/LaTeXML/">LaTeXML <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAsAAAAOCAYAAAD5YeaVAAAAAXNSR0IArs4c6QAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAALEwAACxMBAJqcGAAAAAd0SU1FB9wKExQZLWTEaOUAAAAddEVYdENvbW1lbnQAQ3JlYXRlZCB3aXRoIFRoZSBHSU1Q72QlbgAAAdpJREFUKM9tkL+L2nAARz9fPZNCKFapUn8kyI0e4iRHSR1Kb8ng0lJw6FYHFwv2LwhOpcWxTjeUunYqOmqd6hEoRDhtDWdA8ApRYsSUCDHNt5ul13vz4w0vWCgUnnEc975arX6ORqN3VqtVZbfbTQC4uEHANM3jSqXymFI6yWazP2KxWAXAL9zCUa1Wy2tXVxheKA9YNoR8Pt+aTqe4FVVVvz05O6MBhqUIBGk8Hn8HAOVy+T+XLJfLS4ZhTiRJgqIoVBRFIoric47jPnmeB1mW/9rr9ZpSSn3Lsmir1fJZlqWlUonKsvwWwD8ymc/nXwVBeLjf7xEKhdBut9Hr9WgmkyGEkJwsy5eHG5vN5g0AKIoCAEgkEkin0wQAfN9/cXPdheu6P33fBwB4ngcAcByHJpPJl+fn54mD3Gg0NrquXxeLRQAAwzAYj8cwTZPwPH9/sVg8PXweDAauqqr2cDjEer1GJBLBZDJBs9mE4zjwfZ85lAGg2+06hmGgXq+j3+/DsixYlgVN03a9Xu8jgCNCyIegIAgx13Vfd7vdu+FweG8YRkjXdWy329+dTgeSJD3ieZ7RNO0VAXAPwDEAO5VKndi2fWrb9jWl9Esul6PZbDY9Go1OZ7PZ9z/lyuD3OozU2wAAAABJRU5ErkJggg==" alt="[LOGO]"></a>
</div></footer>
</div> -->
