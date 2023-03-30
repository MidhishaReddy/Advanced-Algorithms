# LRU cache

LRU least recently used object: We will be given a list of value key pairs to add them into the cache and get the key when there is a pop funtion.

This operation of get and put should be done in O(1).&#x20;

For the O(1) complexity to be achieved we think of hash maps and linked list.\
Since the hashmaps are not the ordered list, we will keep track of the order by using the linkedlist datastructure.

We use a doubly linked list, place the newly used element next to the head amd pop it of from the tail.

