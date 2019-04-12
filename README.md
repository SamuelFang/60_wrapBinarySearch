# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

The meaning of y = log2x is 2^y = x. It's graph is an exponential graph reflected over y = x

problem
Find a given index in an ordered list with binary searching

recursive abstraction
To solve the problem, one can find a given index in half of an ordered list with binary searching

decisions
low > hi
comparison == 0

base case solutions
return -2
return pageToCheck

recursive case solutions, combining, recursive abstraction, process leftovers
return indexOf_recursive( findMe , low, pageToCheck -1)
return indexOf_recursive( findMe, pageToCheck +1, hi)