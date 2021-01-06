# Hash Table

* **Hashing** is a technique that is used to uniquely identify a specific object from a group of similar objects

* Assume that you have an object and you want to assign a key to it to make searching easy. To store the key/value pair, you can use a simple array like a data structure where keys (integers) can be used directly as an index to store values. However, in cases where the keys are large and cannot be used directly as an index, you should use hashing.

## Hash function

* **Ahash function** is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

* To achieve a good hashing mechanism, It is important to have a good hash function with the following basic requirements:

  * Easy to compute: It should be easy to compute and must not become an algorithm in itself.

  * Uniform distribution: It should provide a uniform distribution across the hash table and should not result in clustering.

* Less collisions: Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided.

## Hash table

* A hash table is a data structure that is used to store keys/value pairs.
* It uses a hash function to compute an index into an array in which an element will be inserted or searched. By using a good hash function, hashing can work well.
* Under reasonable assumptions, the average time required to search for an element in a hash table is O(1).

## Collision resolution techniques

* **Separate chaining**

  * Separate chaining is one of the most commonly used collision resolution techniques. It is usually implemented using linked lists. In separate chaining, each element of the hash table is a linked list. To store an element in the hash table you must insert it into a specific linked list. If there is any collision

* **Linear probing**
  * In open addressing, instead of in linked lists, all entry records are stored in the array itself. When a new entry has to be inserted, the hash index of the hashed value is computed and then the array is examined (starting with the hashed index).
  * If the slot at the hashed index is unoccupied, then the entry record is inserted in slot at the hashed index else it proceeds in some probe sequence until it finds an unoccupied slot.

  * The probe sequence is the sequence that is followed while traversing through entries. In different probe sequences, you can have different intervals between successive entry slots or probes.

  * When searching for an entry, the array is scanned in the same sequence until either the target element is found or an unused slot is found. This indicates that there is no such key in the table. The name "open addressing" refers to the fact that the location or address of the item is not determined by its hash value.
  * Linear probing is when the interval between successive probes is fixed (usually to 1). Let’s assume that the hashed index for a particular entry is index. 

* **Quadratic Probing**

  * Quadratic probing is similar to linear probing and the only difference is the interval between successive probes or entry slots. Here, when the slot at a hashed index for an entry record is already occupied, you must start traversing until you find an unoccupied slot. The interval between slots is computed by adding the successive value of an arbitrary polynomial in the original hashed index.

  * Let us assume that the hashed index for an entry is index and at index there is an occupied slot.   

## Applications

* Associative arrays: Hash tables are commonly used to implement many types of in-memory tables. They are used to implement associative arrays (arrays whose indices are arbitrary strings or other complicated objects).
* Database indexing: Hash tables may also be used as disk-based data structures and database indices (such as in dbm).
* Caches: Hash tables can be used to implement caches i.e. auxiliary data tables that are used to speed up the access to data, which is primarily stored in slower media.
* Object representation: Several dynamic languages, such as Perl, Python, JavaScript, and Ruby use hash tables to implement objects.
* Hash Functions are used in various algorithms to make their computing faster  
