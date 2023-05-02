Download Link: https://assignmentchef.com/product/solved-comp47670-assignment2-ucd-data-mining
<br>
The objective of this assignment is to scrape a corpus of news stories from a set of web pages, pre-process the data, and evaluate the performance of both binary and multi-label text classification algorithms on the data. The news stories are archived by month at the link below and each story has been assigned one of 9 news categories<em>.</em>

<a href="http://mlg.ucd.ie/modules/COMP41680/assignment2/index.html">http://mlg.ucd.ie/modules/COMP41680/assignment2/index.html</a>

Based on this data, you should complete the three tasks listed below. The assignment should be implemented as a single Jupyter Notebook (not a script file). Your notebook should be clearly documented, using comments and Markdown cells to explain the code and results.

<strong>Task 1. Data Collection</strong>

<ol>

 <li>Select <strong><u>three</u></strong> of the 9 news categories: [Books, Business, Film, Life-and-Style, Music, Politics, Sport, UK-News, US-News]</li>

 <li>From the link above, retrieve details regarding all stories corresponding to your three selected categories, covering all months January to December 2020. For each story you will need to parse the HTML to extract the following information:

  <ol>

   <li>The <em>title</em> of the news story.</li>

   <li>The short <em>text snippet</em> for the story which represents the start of the complete news article.</li>

  </ol></li>

</ol>

<ul>

 <li>The <em>category label</em> assigned to the story.</li>

</ul>

Note: You <strong><u>do not</u></strong> have to retrieve the full linked article from The Guardian, only the data on the mlg.ucd.ie website.

<ol start="3">

 <li>Store the parsed data that you have collected in an appropriate format.</li>

</ol>

<strong>Task 2. Binary Text Classification</strong>

<ol>

 <li>Load the data from Task 1 and create a set of documents, one per news story. Each document should consist of the concatenation of the story’s title and text snippet. Each document should also have a class label, based on the story’s news category.</li>

 <li>For each unique pair of categories (A,B) from the three that you selected:

  <ol>

   <li>Apply appropriate preprocessing steps to create a numeric representation of the documents from these two categories, suitable for classification.</li>

   <li>Train a classification model using a <strong>binary classifier</strong> of your choice, which can distinguish documents in category A from documents in category B.</li>

  </ol></li>

</ol>

<ul>

 <li>Test the predictions of the classification model using an appropriate evaluation strategy. Report and discuss the evaluation results.</li>

</ul>

<strong>Task 3. Multi-Class Text Classification</strong>

<ol>

 <li>Using all three categories (A,B,C) that you have selected:

  <ol>

   <li>Apply appropriate preprocessing steps to create a numeric representation of the documents for these three categories, suitable for classification.</li>

   <li>Train a classification model using a <strong>multi-class classifier</strong> of your choice, which can distinguish documents from the categories A, B, and C.</li>

   <li>Test the predictions of the classification model using an appropriate evaluation strategy. Report and discuss the evaluation results.</li>

  </ol></li>

</ol>