## Heaps 
### max heap
```C++
std::make_heap(); // from a vector to heap
std::push_heap(); // push back 
std::pop_heap(); // swap the first one and the last one and make the heap from 1->(n-1) --> if we want to kill the last one we have to pop_back the vector --> if we want to pop_heap again and again, we sort the heap
```

## Sort
``` C++ 
std::sort   
std:: partial sort 
std:: nth_element //  every in left is smaller and in the right is larger
std::inplace_merge()
```

## Partitioning
```C++
std::parition
std::paritition_point 
``` 
## other permutations
```C++
std::rotation
std::suffle
std::next_permutation
std::prev_permutation
std::reverse
```
## secret runes
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



