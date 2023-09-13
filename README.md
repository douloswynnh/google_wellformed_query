<p class="has-line-data" data-line-start="0" data-line-end="1">Query Wellformedness Model</p>
<p class="has-line-data" data-line-start="2" data-line-end="5">This machine learning project focuses on training a chosen dataset from a Google research dataset called “Google Well-formed Query Dataset” which resulted from crowdsourcing well-formedness annotations for 25,100 queries from the Paralex corpus. Every query sentence was annotated by five raters with a rating of 1/0 whether the query is well-formed or not, i.e. grammatically correct.<br>
<a href="https://github.com/google-research-datasets/query-wellformedness">Dataset link</a><br>
There are three datasets given that have been split into train.tsv, test.tsv, and dev.tsv. We can see a snippet of the dataset:</p>
<table class="table table-striped table-bordered">
<thead>
<tr>
<th>Query Well-formedness rating</th>
<th>Score</th>
</tr>
</thead>
<tbody>
<tr>
<td>The European Union includes how many ?</td>
<td>0.2</td>
</tr>
<tr>
<td>What are Mia Hamms accomplishment ?</td>
<td>0.4</td>
</tr>
<tr>
<td>Mission and vision of amul dairy ?</td>
<td>0.0</td>
</tr>
<tr>
<td>When was the canal de panama built ?</td>
<td>0.8</td>
</tr>
</tbody>
</table>
<p class="has-line-data" data-line-start="13" data-line-end="14">The snippet of the query shows where a sentence is gramatically correct, and explicit question, and if it contains any spelling errors.</p>
<p class="has-line-data" data-line-start="15" data-line-end="16">To train those datasets, a language model that understands English language, is able to connect the context of the question from the start to end, and produce rating based on how the query is well-formed must be used.</p>
<p class="has-line-data" data-line-start="17" data-line-end="18">Transformer models fit the requirements as they can understand sequence of words in a sentence and a little bit of fine-tuning to the model would yield results with great accuracy.</p>
<p class="has-line-data" data-line-start="19" data-line-end="25">@InProceedings{FaruquiDas2018,<br>
title = {{Identifying Well-formed Natural Language Questions}},<br>
author = {Faruqui, Manaal and Das, Dipanjan},<br>
booktitle = {Proc. of EMNLP},<br>
year = {2018}<br>
}</p>
