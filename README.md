Download Link: https://assignmentchef.com/product/solved-prolog-assignment2-more-list-processing-problems-and-cut
<br>
<u>Write PROLOG programs:</u>

<ol>

 <li>To add an element to a list provided it is not present in the list.</li>

 <li>To delete first occurrence of an element from a list.</li>

 <li>To delete all occurrences of an element from a list.</li>

 <li>To replace the first occurrence of an element X in L with Y giving the result in L1.</li>

 <li>has_duplicate(L), that determines whether list L has duplicate elements.</li>

 <li>To duplicate the elements of a list. Example:</li>

</ol>

?- duplicate([a,b,c,c,d],X).

{X = [a,a,b,b,c,c,c,c,d,d]}

7, To duplicate the elements of a list a given number of times.

Example:

?- duplicate2([a,b,c],3,X).

{X = [a,a,a,b,b,b,c,c,c]}




What are the results of the goal:

?- duplicate2(X,3,Y).




<ol start="8">

 <li>To determine whether a list is a sub list of another list. A list is a sub list of another list if it’s elements are present in another list consecutively and in the same order.</li>

 <li>To determine whether a set is a subset of another set.</li>

 <li>To determine intersection of two sets.</li>

</ol>

12.To determine union of two sets.

13.To determine difference of two sets.

14.To determine symmetric difference of two sets.

<ol start="15">

 <li>To replace n th element by another element X in L, leaving the resultant list in L1.</li>

 <li>to remove every N’th element from a list. Example:</li>

</ol>

?- remove([a,b,c,d,e,f,g,h,i,k],3,X).

{X = [a,b,d,e,g,h,k]}




For the problems 17 – 18 assume L1, L2 and L denote lists of terms.

<ol start="17">

 <li>Interleave alternate elements of L1 and L2 into L. For example, if L1= [a, b, c] and L2= [1, 2], then L= [a, 1, b, 2, c].</li>

</ol>

18.Transpose L1, L2 into L. That is, if L1= [a, b, c] and L2= [1, 2, 3], then L= [(a, 1), (b, 2), (c, 3)].

<ol start="19">

 <li>To split a list into two parts; the length of the first part is given. Do not use any predefined predicates.</li>

</ol>




Example:

?- split([a,b,c,d,e,f,g,h,i,k],3,L1,L2).

{L1 = [a,b,c], L2 = [d,e,f,g,h,i,k]}




<ol start="20">

 <li>To extract a slice from a list.</li>

</ol>

Given two indices, I and K, the slice is the list containing the elements between the I’th and K’th element of the original list (both limits included). Start counting the elements with 1.




Example:

?- slice([a,b,c,d,e,f,g,h,i,k],3,7,L).

{X = [c,d,e,f,g]}




<ol start="21">

 <li>To insert an element at a given position into a list.</li>

</ol>

Example:

?- insert_at(alfa,[a,b,c,d],2,L).

{L = [a,alfa,b,c,d]}




For the problems 22 – 30 assume L and L1 is a list of terms.

<ol start="22">

 <li>To remove_every_other (L, L1). List L1 is just list L with every other element removed (the two lists should have the same first element).</li>

 <li>cutlast (L, L1) that defines L1 to be obtained from L with last element removed.</li>

 <li>trim (N, L, L1) that defines L1 to be obtained from L with first N elements removed.</li>

</ol>

25.trimlast (N, L, L1) that defines L1 to be obtained from L with last N elements removed.

26.exchange_first_last(L, L1), defines that L1 to be obtained from L with first and last elements exchanged.

Example:

?-exchange_first_last([a, b, c, d, e], X).

{X= [e, b, c, d, a]}

27 circular_left_shift(L, L1). That is, if L= [a, b, c, d, e, f] then L1= [b, c, d, e, f, a]..

<ol start="28">

 <li>circular_right_shift(L, L1). That is, if L= [a, b, c, d, e, f] then L1= [f, a, b, c, d, e]</li>

</ol>

[Try using circular_left_shift in 27 to implement circular_right_shift.]

29.To delete the middle element from an odd-numbered list L into a list L1.

30.To delete two middle elements from an even-numbered list L into a list L1.