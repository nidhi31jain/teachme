# Collections Framwork
    - Group of elements
    - Provides useful data structures and algorithms

 * Iterable (Interface)
   *  Collection (Interface) extends Iterable
     * List (Interface) extends Collection
       * ArrayList (Class) implements List
       * LinkedList (Class) implements List
     * Set
       * HashSet (Class)
       * SortedSet extends HashSet implements Set
         * TreeSet (Class) extends HashSet implements SortedSet
 
* Map (Interface)
  * HashMap (Interface) extends Iterable
    * SortedMap (Interface) extends HashMap implements Map
    * TreeMap (Class) extends HashMap implements SortedMap
       
[Reference](https://www.novixys.com/blog/wp-content/uploads/2017/02/Collections-768x480.png)

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
