---
keywords: fastai
description: My own quiz with my own questions and Mr. Mortensen's questions.
title: Python Quiz and Hacks
toc: true
badges: false
comments: true
author: Kaiden Do
categories: [python, week1]
image: /images/pythonlogo.png
nb_path: _notebooks/2022-08-26-Python-Hacks.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-08-26-Python-Hacks.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="My-Quiz">My Quiz<a class="anchor-link" href="#My-Quiz"> </a></h2><p>This quiz defines two functions for asking questions and receiving an answer. The quiz has 7 questions. Each question asked is compared to a correct answer and if they are equal (with no regard to case) then the quiz tells the user. If not, then the quiz tells the user that the answer is wrong. The program stores each correct answer and tells the user the percentage of correct answers at the end of the quiz.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">getpass</span><span class="o">,</span> <span class="nn">sys</span> <span class="c1"># imports functions and libraries</span>

<span class="k">def</span> <span class="nf">question_and_answer</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span> <span class="c1"># defines the question_and_answer function</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span> <span class="c1"># asks the user a question</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span> <span class="c1"># takes the user&#39;s input</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Answer: &quot;</span> <span class="o">+</span> <span class="n">msg</span><span class="p">)</span> <span class="c1"># prints the answer and the user&#39;s input</span>

<span class="k">def</span> <span class="nf">question_with_response</span><span class="p">(</span><span class="n">prompt</span><span class="p">):</span> <span class="c1"># defines the question_with_response function</span>
    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Question: &quot;</span> <span class="o">+</span> <span class="n">prompt</span><span class="p">)</span> <span class="c1"># asks the user a question</span>
    <span class="n">msg</span> <span class="o">=</span> <span class="nb">input</span><span class="p">()</span> <span class="c1"># takes the user&#39;s input</span>
    <span class="k">return</span> <span class="n">msg</span> <span class="c1"># the function returns the user&#39;s response as a string value</span>

<span class="n">questions</span> <span class="o">=</span> <span class="mi">7</span> <span class="c1"># number of questions in the quiz</span>
<span class="n">correct</span> <span class="o">=</span> <span class="mi">0</span> <span class="c1"># amount correct in the beginning of the quiz</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Hello, &#39;</span> <span class="o">+</span> <span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; running &quot;</span> <span class="o">+</span> <span class="n">sys</span><span class="o">.</span><span class="n">executable</span><span class="p">)</span> <span class="c1"># greets the user</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;You will be asked &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span> <span class="o">+</span> <span class="s2">&quot; questions.&quot;</span><span class="p">)</span> <span class="c1"># tells the user how many questions are in the quiz</span>
<span class="n">question_and_answer</span><span class="p">(</span><span class="s2">&quot;Are you ready to take a test?&quot;</span><span class="p">)</span> <span class="c1"># prompts the user to start the quiz</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to include other functions that were previously developed?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;import&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What command is used to evaluate correct or incorrect response in this example?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;if&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;expression&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What does &#39;def&#39; do in Python in relation to a function: It _______ the function?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;defines&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What does the function take as a parameter?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;prompt&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;Can static text change?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;no&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="n">rsp</span> <span class="o">=</span> <span class="n">question_with_response</span><span class="p">(</span><span class="s2">&quot;What is the first thing that beginner programmers usually print?&quot;</span><span class="p">)</span> <span class="c1"># asks question and stores the user&#39;s response</span>
<span class="k">if</span> <span class="n">rsp</span><span class="o">.</span><span class="n">lower</span><span class="p">()</span> <span class="o">==</span> <span class="s2">&quot;hello world&quot;</span><span class="p">:</span> <span class="c1"># compares the user&#39;s response to the answer without regard to the case</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is correct!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is correct</span>
    <span class="n">correct</span> <span class="o">+=</span> <span class="mi">1</span> <span class="c1"># one more correct answer</span>
<span class="k">else</span><span class="p">:</span> <span class="c1"># if not correct</span>
    <span class="nb">print</span><span class="p">(</span><span class="n">rsp</span> <span class="o">+</span> <span class="s2">&quot; is incorrect!&quot;</span><span class="p">)</span> <span class="c1"># shows that it is incorrect</span>

<span class="nb">print</span><span class="p">(</span><span class="n">getpass</span><span class="o">.</span><span class="n">getuser</span><span class="p">()</span> <span class="o">+</span> <span class="s2">&quot; you scored &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">correct</span><span class="p">)</span> <span class="o">+</span><span class="s2">&quot;/&quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">questions</span><span class="p">)</span><span class="o">+</span><span class="s2">&quot; or &quot;</span><span class="o">+</span><span class="nb">str</span><span class="p">((</span><span class="n">correct</span><span class="o">/</span><span class="n">questions</span><span class="p">)</span><span class="o">*</span><span class="mi">100</span><span class="p">)</span><span class="o">+</span><span class="s2">&quot;%&quot;</span><span class="p">)</span> <span class="c1"># tells the user how many questions they got correct out of the total questions and their score</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>Hello, kaiden_do running /bin/python3
You will be asked 7 questions.
Question: Are you ready to take a test?
Answer: yes
Question: What command is used to include other functions that were previously developed?
import is correct!
Question: What command is used to evaluate correct or incorrect response in this example?
if is correct!
Question: Each &#39;if&#39; command contains an &#39;_________&#39; to determine a true or false condition?
expression is correct!
Question: What does &#39;def&#39; do in Python in relation to a function: It _______ the function?
defines is correct!
Question: What does the function take as a parameter?
prompt is correct!
Question: Can static text change?
no is correct!
Question: What is the first thing that beginner programmers usually print?
hello world is correct!
kaiden_do you scored 7/7 or 100.0%
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

