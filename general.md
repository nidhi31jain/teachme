# Collections Framwork
    - Group of elements
    - Provides useful data structures and algorithms

 * Iterable
   *  <font color='red'>Collection</font>
     * <span style="color:blue">AbstractCollection</span>
     * <span style="color:red">List</span>
       * <span style="color:green">ArrayList</span>
       * <span style="color:green">LinkedList</span>
     * <span style="color:red">Set</span>
     * <span style="color:blue"></span>
       * <span style="color:green">HashSet</span>
## Collection Interface
  * size
  * isEmpty
  * add
  * remove
  * iterator

  * addAll - union
  * removeAll - subtraction
  * retainAll - intersection
  * clear
  
 * Iterator
    *# hasNext
    *# next
    *# Remove
    
Set Interface - Cannot contain duplicate elements - HashSet(default 16 size) , TreeSet , LinkedHashSet

## List - Ordered collection - ArrayList , LinkedList
- Positional Access
- ListIterator
- sort
- binary search

## Queue - LinkedList
Throws exception
- add
- remove
- element
Returns special value
- offer
- poll
- peek
## DeQueue - LinkedList
- all operations of Queue at the begining and end
## Map - Key and values - HashMap , TreeMap , LinkedHashMap
- Collection Views
  - Keyset
  -Values
  -Entryset(to iterate over a Map)
SortedSet
SortedMap - Keys in sorted Order
SynchronizedWrappers
  Interface.synchronizedXXX
UnmodifiableWrappers
  Interface.unmodifiableXXX
