# comp47470-project-2-solved
**TO GET THIS SOLUTION VISIT:** [COMP47470 Project 2 Solved](https://www.ankitcodinghub.com/product/comp47470-project-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95399&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP47470 Project 2 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
1 Hadoop

In this section you will run Hadoop MapReduce jobs on a dataset of shuttle trips. Download the data using the following code (remember to make it all one line!):

<pre>    wget --no-check-certificate
</pre>
<ul>
<li>􏰀→ &nbsp;‘https://docs.google.com/uc?export=download&amp;id=1Jvw6rGC8X8H7bDXzSiP4mf2Q_wyOFWs2’</li>
<li>􏰀→ &nbsp;-O shuttle.csv</li>
</ul>
<ol>
<li>How many rides occurred per weekday?</li>
<li>Using a mapreduce operation, count the number of rows in the dataset</li>
<li>What was the most common number of passengers?</li>
<li>How many rides (grouped per day) had a total amount greater than 20?</li>
<li>How many trips occurred on weekdays?</li>
<li>How many trips occurred before 2pm? (you may include/exclude 2pm – just be con- sistent!)</li>
<li>What is the average ”fare amount” per day . You may use a combination of mapreduce output and bash scripting to accomplish this (e.g. two separate mapreduce tasks with a small bash script ”combining” the two outputs). For the purposes of this assignment, you can assume that the fare will be an integer between 0 and 9.</li>
</ol>
1.1 Notes:

<ul>
<li>This section can be completed by modifying the ”WordCount” example provided to you in Lab 4. Please look at the solutions document for that lab to orient yourself. You will be editing the WordCount file and compiling it inside your docker container – this will limit your debugging potential so it may be preferable to test some changes in a separate Java environment before inputting them (see the last point below).</li>
<li>The majority of modifications will be made in the TokenizerMapper class (hint: look at the context.write() and word.set() functions) and the IntSumReducer class (take a look at the code after ”public void reduce”).</li>
<li>Please remember to look at the Hadoop documentation – many of the functions will not accept strings/integers, and will instead require the creation of new variables of the appropriate type – e.g. in the context.write() function in the TokenizerMapper class, the number ”one” is not an integer or a string – it is an ”IntWritable” – if we wanted to modify this write to include a different integer (using 7 as an example), we would have to make a new IntWritable as so: ”IntWritable t1 = new IntWritable(7);” and include this in the write: ”context.write(word, t1);. Similarly the ”key” variable in IntSumReducer is not a string, but a ”Text” item that can be constructed similarly. This information is available in the code, but might require a close reading!</li>
<li>The following resource may be useful to you: MapReduce Tutorial</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Page 2 of – 5

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
COMP47470 Project 2

</div>
</div>
<div class="layoutArea">
<div class="column">
• You may find it helpful to create a smaller dataset to probe functionality on! Alter- natively, you might require a Java IDE to test some specific functionality – if you do not have Java on your system, there are some basic implementations available online – see here

2 Spark

For this section, you will be assessing a dataset of Netflix shows. Download the data using the following code (remember to make it all one line!):

<pre>    wget --no-check-certificate
</pre>
<ul>
<li>􏰀→ &nbsp;‘https://docs.google.com/uc?export=download&amp;id=1qzTZflrsZ89dYPct3KpFO0O9LmrN2yck’</li>
<li>􏰀→ &nbsp;-O netflix.csv
Launch the Spark shell and then create an RDD or a DataFrame from the input file. For each of the following tasks, write Scala code to solve it. You can use operations on DataFrames (see lab 5 and here, in the Scala API, DataFrame is simply a type alias of Dataset[Row]), spark SQL on Dataframes (see lab 5), or operations on RDDs (see lab 5, here, and here).
</li>
</ul>
<ol>
<li>How many rows are in the dataset?</li>
<li>Are there more TV Shows or Movies in the dataset?</li>
<li>Compute the total duration for each type (Movie/TV Show) in the dataset. You may disregard the season/minute distinction for this question.</li>
<li>What is the oldest (by release year) movie in the dataset?</li>
<li>Determine the number of movies per country. Some country fields will contain multiple countries delimited by a semicolon.</li>
<li>Determine the most frequently occurring term in the the ”description” field (i.e what word appears the most often in that column!)</li>
<li>To the nearest decade (e.g. 2000-2009 == 2000s), what are the top 5 decades in terms of number of films released.</li>
<li>In what month have the most films been added to Netflix (i.e. sum of all the films added in a given month)</li>
</ol>
2.1 Notes:

<ul>
<li>Remember to check your ”pipeline” if you are receiving unexpected errors – Scala is very precise, so make sure you know what is being passed from each function to the next – it may not be what you think! A good example is during the mapping process – repeated maps (e.g. when splitting on successive dividers) can often lead to nested arrays (rather than an expected single level array!). As a hint, think about what flatMap( .toList). might do in a situation like this!</li>
<li>Don’t be afraid to do outside research for this section – and especially make sure to look at the documentation linked above for functions etc. – but you shouldn’t require anything too distant from what you have already completed in the labs!</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column"></div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea"></div>
<div class="layoutArea">
<div class="column">
• Simplicity is key – try to avoid creating complex structures (e.g. an array of arrays of STRING,INT …) where possible. It will be less frustrating for you, and will speed up the process of creating a solution.

3 Reflection

Please complete both of the following two titles: 3.1 Topic 1 – Spark and Hadoop

Write a short report (max. 2 pages) exploring the following topic: ”Spark &amp; Hadoop: Advantages and drawbacks of each technology, and why you might choose one over the other”. Your discussion should address the following topics:

• A brief overview of the two technologies

• What the major technical differences are between Spark and Hadoop • In what circumstances would you choose Spark over Hadoop

• In what circumstances would you choose Hadoop over Spark

You are expected to cite at least one paper in your answer, in addition to any web/al- ternative resources that you use. You may use a citation style of your choice, as long as you are consistent! Two papers (concerning Spark/RDDs and Hadoop/HDFS) are available on Brightspace to help you orient yourself – you may use these to fulfil the paper requirement (but you are not limited to using only them!).

3.2 Topic 2 – Paper Review

Write a short report (max. 2 pages) on one of the research papers that are available on Brightspace. The following list of sections is an indication of how to write your paper. Some of the items might not be relevant for all papers, and you might want to add some sections in your report (e.g. evaluate the posterity of a solution etc.). We will have an open mind when reading your report and we just want to see how you analyse a research paper and are able to discuss it – in short there is no one single perfect report, everything that shows you made an effort to understand and focus on the important parts (research methodology, hypotheses, etc.) will be welcome.

<ul>
<li>identify the question/challenge the paper addresses. Explain in your own words what the motivation for the research is.</li>
<li>describe briefly the related work, i.e., the other (related) solutions that the authors compare themselves to. Show the limitations of these related solutions</li>
<li>Give an outline of the solution proposed by the authors (no need to go into details) showing the main components</li>
<li>describe their scientific method: what are the research questions they evaluate, how do they evaluate</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column"></div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea"></div>
<div class="layoutArea">
<div class="column">
• describe briefly their results

• give your impression on the idea, what you liked about the paper and whether you see any limitations etc.

</div>
</div>
</div>
