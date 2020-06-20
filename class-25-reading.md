[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 25: DSA: HashTables

### Links

- [What is a HashTable Data Structure?](https://www.youtube.com/watch?v=MfhjkfocRR0) 
- [Basics of HashTables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/) 
- [HashTable - Wikipedia](https://en.wikipedia.org/wiki/Hash_table) 
                                              

### Discussion Questions:

#### 1. Is a HashTable useful for search or sorting operations? Why? 
It's used to store information. It is useful for searching operations because data is stored in an array format, where each data value has its own unique index value. Access of data becomes very fast if we know the index of the desired data.

#### 2. What makes a good hash function? 
It's easy to compute, uniform distribution, and less collisions. The bigger it is the better for performance.

#### 3. Why should you try to reduce the number of collisions?
To maintain the performance of the hash table.

#### 4. What is stored at each index of a HashTable? Why?
Value is stored at each index of a HashTable. A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

