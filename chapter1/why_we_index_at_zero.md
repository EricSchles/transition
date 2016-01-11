#Why we index at zero - an intuitive explanation

So when we learn sets in computer science, we index starting at zero.  Why?

To understand this, I'm going to introduce a concept called cardinality:


__Intuitive__ __Definition__ **Cardinality** := The cardinality of a finite set is the total count of all it's elements.

Thus, the set A = [2,3,4] has a cardinality of 3, written |A| = 3.  For real numbers, this is equivalently, the absolute value of a number.

But wait!

How can [2,3,4] have cardinality of 3 and the distance from 2 to 4 have a length of 2?

Doesn't this open us up to a lot of problems?

Like - |[2,3,4]| + |[5,6,7,8]| = 7 but 8-2 = 6.

So we'll be off by one if we want to count ordered sets.  That sucks!  One of the ways around this is:

Index your set at zero!  So:

[2,3,4,5,6,7,8]

 ^ ^ ^ ^ ^ ^ ^
 
 0,1,2,3,4,5,6

 Then "discrete distance" (our cardinality) and our "continuous distance" (distance over the reals since it's a space with a metric) match up!

