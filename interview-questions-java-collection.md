# Collections Framwork
    - Group of elements
    - Provides useful data structures and algorithms

 * Iterable (Interface)
   *  Collection (Interface) extends Iterable
      * List (Interface) extends Collection
        * ArrayList (Class) implements List
        * LinkedList (Class) implements List
      * Set
        * HashSet (Class) implements Set
        * SortedSet extends HashSet implements Set
          * TreeSet (Class) extends HashSet implements SortedSet
       
[Reference](https://www.novixys.com/blog/wp-content/uploads/2017/02/Collections-768x480.png)

#### Collection Interface methods
* size
* isEmpty
* add
* remove
* iterator
* addAll - union
* removeAll - subtraction
* retainAll - intersection
* clear

#### List(Interface) - Ordered collection - ArrayList(Class) , LinkedList(Class)
- binary search
- Positional Access using index
- ListIterator specically designed for list to iterate item from list 
- sort
#### Queue - LinkedList
Throws exception
- add
- remove
- element
Returns special value
- offer
- poll
- peek
#### DeQueue - LinkedList
- all operations of Queue at the begining and end

#### Iterator Interface methods

* hasNext
* next
* Remove
    
Set Interface - Cannot contain duplicate elements - HashSet(default 16 size) , TreeSet , LinkedHashSet

## Map - Key and values - HashMap , TreeMap , LinkedHashMap
* Map (Interface)
  * HashMap (Interface) extends Iterable
    * SortedMap (Interface) extends HashMap implements Map
    * TreeMap (Class) extends HashMap implements SortedMap

* Collection Views
  - Keyset
  - Values
  - getKey(key)
  - Entryset(to iterate over a Map)
  
SortedSet
SortedMap - Keys in sorted Order
SynchronizedWrappers
  Interface.synchronizedXXX
UnmodifiableWrappers
  Interface.unmodifiableXXX
