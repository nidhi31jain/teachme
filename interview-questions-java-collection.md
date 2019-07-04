# Collections Framwork [Reference](https://www.novixys.com/blog/wp-content/uploads/2017/02/Collections-768x480.png)
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
       


#### Collection Interface methods
```
- int size() 
- boolean isEmpty() return true/(boolean) if collection is empty else false 
- boolean add(Object object)
- void add(index, Object object)
- boolean remove(Object object)
- Iterator iterator()  return a Iterator object 
- addAll(Collection collection) - union of two collection to one - list.addAll(otherlist)
- remove(Object object) - subtraction
- removeAll(Collection collection) - subtraction
- retainAll() - intersection
- clear
```

#### List(Interface) - Ordered collection - ArrayList(Class) , LinkedList(Class)
- binary search
- Positional Access using index
- ListIterator specically designed for list to iterate item from list 
- sort
#### Queue - LinkedList
Throws exception
``` 
- add
- remove
- element
```
Returns special value
```
- offer
- poll
- peek
```
#### DeQueue - LinkedList
- all operations of Queue at the begining and end

## Iterator Interface methods
```
- boolean hasNext() 
- Object next()
Remove

List<String> listString = new ArrayList<>();
Iterator iterator = list.iterator()
while(iterator.hashNext()){
    String value = (String)iterator.next();
    //TODO the rest
}
```    
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
