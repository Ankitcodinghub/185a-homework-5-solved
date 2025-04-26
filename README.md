# 185a-homework-5-solved
**TO GET THIS SOLUTION VISIT:** [185A Homework 5 Solved](https://www.ankitcodinghub.com/product/185a-homework-5-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91031&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;185A Homework 5 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Instructions: Download FiniteState.hs and Assignment05.hs from the course website into the same directory on your computer. The import line near the top of Assignment05.hs imports all of the definitions from FiniteState.hs, which you may then use in your assignment. Please submit your assignment as one file: a modified version of Assignment05.hs.

 10 points A strictly-local grammar (SLG) is an alternative to an FSA. Like an FSA, an SLG

generates a set of strings over some alphabet:

(1) A strictly-local grammar is a four-tuple ⟨, S, F, T⟩ where: a. , the alphabet, is a finite set of symbols;

b. S ⊆  is the set of allowable starting symbols;

c. F ⊆  is the set of allowable final symbols; and

d. T ⊆  ×  is the set of allowable two-symbol sequences (called “bigrams”). For an SLG to generate a string of n symbols x1x2 . . . xn , the following must hold:

(i)x1 ∈S,(ii)xn ∈F,and(iii)foralli∈{2,…,n},(xi1,xi)∈T.

For any type sy which our chosen symbols belong to, an SLG can be straightfor- wardly represented in Haskell as a tuple with the following type (technically, a type alias):

</div>
</div>
<div class="layoutArea">
<div class="column">
Ethan Poole ling 185a: Comp. Ling. I Due: 7 May 2019

</div>
</div>
<div class="layoutArea">
<div class="column">
(2) type SLG sy = ([sy], [sy], [(sy,sy)])

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 1 of 5

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
Two examples using this type are given below in (3). The SLG in (3a) has SegmentCV as its symbol type and generates all strings consisting of one or more Cs followed by one or more Vs. The SLG in (3b) has Int as its symbol type and generates all strings built out of the symbols 1, 2 and 3, which do not have adjacent occurrences of 2 and 3 (in either order). These two SLGs are defined in FiniteState.hs with the names slg1 and slg2 respectively.

(3) a. ([C], [V], [(C,C),(C,V),(V,V)])

b. ([1,2,3], [1,2,3], [(1,1),(2,2),(3,3),(1,2),(2,1),(1,3),(3,1)])

Task: Please write a function recognizeSLG that checks whether a given string of symbols is generated by a given SLG:

</div>
</div>
<div class="layoutArea">
<div class="column">
(4) a.

</div>
<div class="column">
Type signature:

</div>
</div>
<div class="layoutArea">
<div class="column">
recognizeSLG :: (Ord sy) =&gt; SLG sy -&gt; [sy] -&gt; Bool b. Example usage:

􏰍⇒ True 

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognizeSLG slg1 [C,C,V]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognizeSLG slg1 [V,C]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognizeSLG slg2 [1,2,1,2,1,3]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
􏰍⇒



􏰍⇒

</div>
<div class="column">
􏰍⇒ True 􏰍⇒ False

</div>
</div>
<div class="layoutArea">
<div class="column">
False

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognizeSLG slg2 [1,2,1,2,1,3,2]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognizeSLG slg2 []
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
False

</div>
</div>
<div class="layoutArea">
<div class="column">
Any string set that can be generated by an SLG can also be generated by some FSA. We know this because for any SLG, there is a mechanical recipe for constructing an FSA that generates exactly the same string set (though not vice versa). Part of your task is to figure out what this recipe is—which you should be able to do from (5) and (6): applying the recipe to the SLG in (3a) produces the FSA in (5), and applying the recipe to the SLG in (3b) produces the FSA in (6).

Page 2 of 5

</div>
</div>
<div class="layoutArea">
<div class="column">
2 10 points

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
(5)

(6)

</div>
<div class="column">
CV

CV

2 12

2

1 3

</div>
</div>
<div class="layoutArea">
<div class="column">
1 31

3

</div>
</div>
<div class="layoutArea">
<div class="column">
Task: Please write a function slgToFSA that takes as input an SLG and produces an FSA. Note that the Automaton type in FiniteState.hs has been simplified so that it does not use ‘record’ syntax; it is just an ordinary tuple now.

What is the type of slgToFSA? Its input can be an SLG with any type as its symbol type. Remember that our FSA type has two “type parameters”: a type for its symbols and a type for its states. Working out the symbol type of the output FSA is easy: this will be the same as the symbol type for the SLG. For the state type of the output FSA—an SLG has no states after all—, you should use the type ConstructedState sy (where sy is whatever type the given SLG’s symbols are):

(7) data ConstructedState sy = ExtraState | StateForSymbol sy

Page 3 of 5

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Putting all of this together, the type of slgToFSA is thus:

(8) slgToFSA :: SLG sy -&gt; Automaton (ConstructedState sy) sy

You may test your function using recognize: recognize (slgToFSA g) x should give the same result as recognizeSLG g x, for any SLG g and any string x.

3 10 points Please write a function reToFSA that converts regular expressions to FSAs. You

should break this task up into two parts.

First, you should write the functions unionFSAs, concatFSAs, and starFSA, with the following types:

(9)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
unionFSAs :: (Ord sy) =&gt; EpsAutomaton Int sy

-&gt; EpsAutomaton Int sy -&gt; EpsAutomaton Int sy

concatFSAs :: (Ord sy) =&gt; EpsAutomaton Int sy

-&gt; EpsAutomaton Int sy -&gt; EpsAutomaton Int sy

starFSA :: (Ord sy) =&gt; EpsAutomaton Int sy -&gt; EpsAutomaton Int sy

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
These three functions should implement the recipes for constructing new -FSAs out of existing -FSAs, which we need in order to implement the overall recipe for constructing an -FSA out of a regular expression, as described in the class handout on -FSAs.

Second, those three functions should be used as part of the definition of reToFSA:

Page 4 of 5

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
(10)

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
reToFSA :: (Ord sy) =&gt; RegExp sy -&gt; EpsAutomaton Int sy reToFSA (Lit x) = …

reToFSA (Alt r1 r2) =

unionFSAs (reToFSA r1) (reToFSA r2) reToFSA (Concat r1 r2) =

concatFSAs (reToFSA r1) (reToFSA r2) reToFSA (Star r) = starFSA (reToFSA r) reToFSA ZeroRE = …

reToFSA OneRE = …

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Putting all of this together should have the following behavior:

(11) 􏰍⇒ True 􏰍⇒ False

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re2)) "acacbcac"
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re2)) "acacbca"
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re3)) []
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re3)) [3]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
False

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re4)) [0,2,2,2]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re4)) [1,2,2]
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>recognize (removeEpsilons (reToFSA re4)) [0,1,2,2,2,2,2]
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
􏰍⇒ True 

􏰍⇒

􏰍⇒ True

To help you out, I have provided the helper function ensureUnused. Given a list of “reserved” integers and an FSA that uses integers for its states, this function produces a new equivalent FSA that is guaranteed not to use any of the reserved integers for its states. While it is not important exactly how this function works, it will be useful on this part of the assignment because if you want to “include” an FSA in a larger FSA à, you need to make sure that the states of are kept distinct from all the other states in à.

</div>
</div>
</div>
