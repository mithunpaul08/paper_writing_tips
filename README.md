

# Common issues seen in the lab while writing a research article

Needless to say, writing a research article is a big part of your graduate work. This document aims to provide guidance on the common issues your advisors have seen in this process. This is by no means a complete document; it will grow as we see issues popping up. So please come back often. 
Last edit: March 2020

## 1. Paper structure

### Overall structure

The most common structure for an empirical NLP paper in CS (but by no means the only one!) is this:
1. Introduction: summary of what your paper is about (see below for details)
2. Related work: how your work builds on and compares against previous work. Summarize what is relevant, and, for each class of papers discussed, explain how your work is different and, ideally, better.
3. Approach: description of your approach. This is the place to be technical.
4. Experimental setup: describe how you evaluated your method. Include a description of the dataset(s) used, baselines, and any practical details that are important (e.g., how you tuned the parameters in your model). 
6. Discussion of results: list the results you measured, and discuss what they mean.
7. Conclusion: take home message.

### Abstract
-   If you use percentages always mention if they are  are relative or absolute
-   s

### Introduction

Very often, the hardest section to write is the Introduction. Because of this, I recommend following this strict structure (at least until you are comfortable with your writing skills):
1. First paragraph: what problem are you working on. Why is it important, and why is it hard.
2. Second paragraph: a summary of your contribution in plain English. This paragraph should be understandable to a scientist that may not be exactly in your field. Thus, minimize NLP/ML jargon as much as possible. 
3. Third paragraph (optional): a more technical description of the paper, if the above paragraph was not sufficient to explain why your work is so cool. This is to get the NLP readers excited about your work. 
4. Contributions: an itemized list of the contributions of this paper. Make this as specific as you can, so it is crystal clear to anybody who reads it what the contribution of this work is. Aim for around three items here.
5.Don't bury the lede- Get to your point in the first page itself.
6. Don’t include an overview section in the intro section for an 8 page long paper. Same for conference presentations, you don’t need an overview slide.


### Related work
- Start with related work/prior art search even before you start to code. You don't want to re-invent the wheel.
- Also this helps for scoops: situations where something very similar to your work was just published by someone else. This happens a lot when you are trying to beat a leaderboard.

### Results
- Don't just say one line about your results. Try to explain why the results are different between the systems.
- Don’t make up a nice story if you cant support it with results. Just be honest
- Include an ablation test i.e remove one contribution at a time.
- Your approach/contribution can be a collection of things. Its ok that one alone is not great, but is combinedly great.

### Figures
- The captions of your figures must be self contained. i.e if a reviewer is going to read ONLY your captions (and not the paper in detail) he should still be able to get a rough idea of what that figure/table is about.

### References
- Try to use bibtex
- Try to use reference from the proceedings of a well known conference, instead of from arxiv if possible. Gives more authenticity and saves the reviewer the pain of confirming the importance of the reference.

As an example, a paper that follows this structure is here: https://www.aclweb.org/anthology/K17-1009 

## 2. Common phrases

1. "System" vs. "method": In a research paper use “approach” or “method” instead of “system”. The former refers to research/scientific ideas; the latter indicates a whole software system, which is usually not the focus in these papers. Using "system" is not only incorrect in most cases, it also may affect you negatively because the reviewer may perceive your work as software development instead of a research contribution. 

2. A “model” is what a method or classifier produces/learn, i.e., its output. For example, if your method relies on deep learning, the model is the set of network weights learned during training. In most of your text, you should use “method/approach” instead of “model” when you discuss your approach. 

3. Idioms: use “off-the-shelf” instead of “off-the-shelves”.

4. Never use "many". Use the exact number or "several". For example, you should say "We analyze and examine the effect of such techniques on several datasets" or "3 datasets" instead of "many datasets".

5. Avoid 'selfish' adjectives. Eg: "well, interesting". An "interesting example" might be interesting to you only, not to others. "Correlates with" is better than "correlates well with".


## 3. Common punctuations and abbreviations

1. Use Oxford commas to reduce the ambiguity in your text. That is, use “A, B, and C” instead of “A, B and C”. See why here: https://en.wikipedia.org/wiki/Serial_comma#Resolving_ambiguity 

2. Use American instead of British spelling. For example, use “analyze” instead of “analyse”.

3. “Eg.” is correctly spelled “e.g.” and is always followed by comma. "E.g." means "exempli gratia" or "for example" in English. Just like you add comma after "for example", you should add a comma after "e.g.".

4. There is always a comma before "etc.". For example: "mammals include dogs, cats, etc."

5. "I.e." is spelled in lower case inside a sentence, and requires commas before and after. "I.e." means "id est" or "that is" or "in other words" in English.

6. Always use commas before "which". In fact, it's good to review the difference in usage and *meaning* of "that" vs. "which": https://www.writersdigest.com/online-editor/which-vs-that

7. The correct spelling for "et al." is what you see here. "Et al." means "et alii" (or "and others" in English). Thus, "alii" is the abbreviated word here.

8. From Jimmy Lin: put footnotes immediately after sentence punctuation not before. For example, this is good placement: "I'm never sick at sea.\footnote{Well, hardly ever.}"

9. There is no comma after "such as". For example, "animals such as dogs and cats". 

10. From Mike Hammond: I find that students are often seduced by using acronyms, easier to type, looks "sciency", etc. For my money, I think that unless they're using an acronym that everybody in the general field uses, this should be really avoided.

11. Always include a white space before a \cite.

## 4. Common spelling mistakes

1. "parenthesis" is singular. "parentheses" is plural. Similarly, "hypothesis" is singular, while "hypotheses" is plural.

2. "data" is plural, "datum" is singular (to refer to a generic item in the set of data).

### 5. Other errors

1. Never ever use an acronym without defining it first. Even if it is something obvious to you like NLP.

2. Do not capitalize words unnecessarily. For example, in the sentence "Social Media has been recognized as...", "Social Media" should *not* be capitalized. Aim to capitalize just names, and acronyms. 

3. Minimize coreference to increase clarity. For example, *It* in the second sentence in this text "For example, XYZ propose a supervised learning approach that ... It tackles several problems..." is fairly ambiguous. When ambiguities exist, please replace the pronouns with a more descriptive noun phrase, e.g., the second sentence in the above example reads better as "The proposed approach tackles several problems..."

- Don't use acronyms in titles
- Expand numerals if they are less than 10 (e.g., use FOUR instead of 4) but not for numbers more than 10. (e.g., 58 is 58 and you don’t need to say “fifty eight”)


### General advice
- Don’t patronize your readers, if you are working on LSTM, don't include a picture of LSTM. However, if you have a new architecture, definitely explain it.
- After working on a paper for a day, put it aside and look at it 2 days later.
- Usually students err at the side of caution, i.e wayyyy too much information. Don't.
- Tuning: Less tuning means you have more confidence in your model. Try to tune the learning rate to the maximum. Even optimizers are optional.
- Technical writing is not literature. People are coming to your paper not to find your literary skills, but to find what you have come up with new.
- Ideas wise you might start with one, and end with other, but thats ok.
- There is a school of thought which even suggests you should write the entire paper before starting to implement it.
- While writing the paper it is a good idea to start with results section (and get it reviewed by your advisor or someone who knows the work). That will give you a clear cut tangible platform to stand/of what the crux of your paper is.
- Always use a segue: don't hit your reader with a sudden change of topic. Ease the reader into why you are changing the topic.
- Always use active voice instead of passive voice. e.g., ``An example can be seen in Table1`` is wrong. use ``We show the example in Table 1``. This shows the reviewer that you are boldly taking up responsibility for your work.
- Don’t make your claims too strong...hedge always (e.g.,use `incorrect` instead of `wrong`. `Wrong` is too strong a word.)
- Don't say ``this is the proof that`` unless you are deriving a mathematical proof. In our line of work `empirical demonstration of the hypothesis` might be a better choice.

### 6. Advice from other people

1. [Novelist Cormac McCarthy’s tips on how to write a great science paper](https://www.nature.com/articles/d41586-019-02918-5)
2. Mihai's [recommended readings on this topic](http://surdeanu.info/mihai/prospective.php) to prospective students. 
3. Google's technical writing course, [part one](https://developers.google.com/tech-writing/one) and [part two](https://developers.google.com/tech-writing/two).
4. [writing samples from clulab](https://github.com/clulab/writing-samples)
