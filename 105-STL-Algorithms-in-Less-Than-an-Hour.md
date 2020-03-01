## Heaps 
### max heap
```C++
std::make_heap(); // from a vector to heap
std::push_heap(); // push back 
std::pop_heap(); // swap the first one and the last one and make the heap from 1->(n-1) --> if we want to kill the last one we have to pop_back the vector --> if we want to pop_heap again and again, we sort the heap
```

## Sort
``` C++ 
std::sort()   
std:: partial sort() 
std:: nth_element() //  every in left is smaller and in the right is larger
std::inplace_merge()
```

## Partitioning
```C++
std::parition()
std::paritition_point() 
``` 
## Other permutations
```C++
std::rotation()
std::suffle()
std::next_permutation()
std::prev_permutation()
std::reverse()
```
## Secret runes
```C++
stable_*   ex : --> stable_sort
           ex : --> stable_partition
is_*       ex:  --> is_sorted
           ex:  --> is_partition
           ex:  --> is_heap
is_*_until ex:  --> is_heap_until
           ex:  --> is_sorted_until
```
## Query
### Numeric algorithm
```C++
std::count() // how many times the value in the clooection
std:: accumulate()/(transform_)reduce // can not only sum the elements together but use some customize transform
std:: partial_sum()/(transform_)inclusive_scan
/ (transform_)exclusive_scan
std:: inner_product()
std:: adjacent_difference()
std:: sample()
```
### Query a property
```C++
std:: all_of() // return with empty collection? True
std:: any_of() // return with empty collection? False
std:: none_of() // return with empty collection? True
```
### Querying a property on 2 ranges
```C++
std:: equal() // retrun bool
std:: mismatch() // find the first position they differ
```
### Searching a value
#### Not sorted array
```C++
std::find() // find the index of that value
std::adjacent_find()// the the position that those two value appear in a row
```
#### Sorted array
```C++ 
std::equal_range()
std::lower_bound()
std::upper_bound()
std::binary_search() // only return the bool
```
#### Searching a range 
```C++
std::search() // searching a subrange into a big range
std:: find_end() // searching from the end
``` 
#### Searching a relative value
```C++
std:: max_element()
std:: min_element()
std:: minmax_element()//retrun a pair of iterator
```
## Set
### any sorted collection (set + sorted array...)
```C++
std:: set_difference() // retrun the element that are in the first one but not in the second one // ;inear complexity
std:: set_intersection()
std:: set_union()
std:: set_symmetric_difference()
std:: include() // return bool whether B is in A or not.
```
## Movers
```C++
std::copy()
std::move()
std::swap_ranges()
std::copy_backward()
std::move_backward()
```
## Value Modifiers
```C++
std:: fill()
std:: generate() // use a function that can be called with no argument
std:: iota() // increment until fill the whole collection
std:: replace() // can replace a value with anothere value
```
## Change structure
```C++
std:: remove() // remove some value but they only move the value to the left and left the empty space
std::erase()
std::unique()// remove the adjacent duplcated in a collection // the end place would also be empty
```
```C++
// the remove unique rotate replace partition partial_sort happened inplace 
// if we want to make a new space, just use *_copy
*_copy  --> ex: remove_copy  
        --> ex: rotate_copy
// 
*_if    --> ex: find_if
```

## Transform
```C++
// input     x1     x2      x3     x4
// output   f(x1)   f(x2)  f(x3) f(x4)
std:: transform()
// can also input 2 collections
// input     x1         x2        x3       x4
// input     y1         y2        y3       y4
// output  f(x1,y1)   f(x2,y2)  f(x3,y3)  f(x4,y4)
```

## for_each
```C++
std::for_each(begin(collection),end(collection),f)
// Collections:   x1     x2     x3    x4
// Calls        f(x1)  f(x2)  f(x3)  f(x4)
// we want the side effects
```

## Raw Memory
fill,copy and move use operator= ,however, sometimes we want to assign them to a raw memory
```C++
std::uninitialized_fill()
std::destroy()
```

## _N
replace the end iterator with size
```C++
std::fill_n()
```