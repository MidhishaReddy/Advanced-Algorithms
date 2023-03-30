# Sliding window

#### Identification:

* Could be an array or string&#x20;
* highlight would the subarray or substring
* Given Window  Size - fixed size, find the max answer or min answer based on the condition.
* Given Condition - variable size, find the max window size or min window size



Sliding window in general helps reduce the nested for loops and solve the problem with in a single for-loop.

When can we use it:\
\-When we need to keep track of the contiguous sequence of elements.\
\-Dealing with subarray of specific length.

There are two types of sliding window problems : \
1\. Fixed size window\
2\. Variable size window\


#### Fixed Size window:&#x20;

General format:

<pre><code>// code skeleton:
<strong>    let k be the window size:
</strong><strong>//let the right and left be two pointers starting at a[0]
</strong><strong>    right=0;
</strong>    left=0;
while(right&#x3C;size){
  //caluculation:
     ......... 
 if(winSize &#x3C; k){
  right ++;
  }
  else if(winSize == k){
  //generate an answer from the caluculations above:
  //remove caluculation of "i" from the current window 
  left++;//To maintain the window size
  }
 }
 return ans;
 }
</code></pre>

#### Variable size window:

Here the size of window is unknow, infact that would be the return value of the question.



```
// Some code
```

Difference between Fixed size and variable size:\
&#x20;

| Fixed size                                   | Variable size               |
| -------------------------------------------- | --------------------------- |
| Window size = given                          | Given condition             |
| we need to get the condition                 | Window size to be maximized |
| easy to move the window , right++ and left++ |                             |
| Hit the window size                          |                             |
|                                              |                             |
