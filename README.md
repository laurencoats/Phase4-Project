# Netflix Recommendation Proposal 
### Presentation and Analysis/Analytics by Lauren Coats

## Overview 
Create recommendation system that will pull movies based on review.  Include a survey to address cold start issue. Use data and intuition to suggest the best model. 
## Business Problem 
Some one accidently deleted Netflix recommendation system gives suggestion to their customers about other shows and movies they would like.  They have hired a Data science consultant that suggest the best recommendation method. 
Data 
Data being used is from the [MovieLens Latest Datasets](https://grouplens.org/datasets/movielens/latest/).  The data set is over 27 million entried long.  For the sake of time and available computing power only 100,000 entries will be used.
## Methods
* SVD
* KNN With Means
* KNN Basic
* KNN Baseline 
## Results 

<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">   <br>Methods   </th>
    <th class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>RSME(AVG)&nbsp;&nbsp;&nbsp;</th>
    <th class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>Fit Time(AVG)&nbsp;&nbsp;&nbsp;</th>
    <th class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>Test Time (AVG)&nbsp;&nbsp;&nbsp;</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>SVD&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.88763&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.82&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.23&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>KNN Basic&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.9520&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.11&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>1.68&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>KNN Baseline&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.8724&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.24&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>2.24&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>KNN with&nbsp;&nbsp;&nbsp;Means&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.9007&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>.14&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br>2.28&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

## Conclusion 
All the models performed well with KNN Basic performing the best based on RSME(AVG). For tis recommendation system SVD will be chosen to because of the low set time. 

## Next Steps 
* Test the models on the full data set 
* Reduce the interval of stars from .5 to 1 to if tere will be an decrease test time  
* See if we can use this code to expand in to other area, ie products, music, ect.
