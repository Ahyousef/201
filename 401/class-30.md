# Hash Tables

## What are they

Hash Tables are a data structure that is an array consisting of pairs of keys:values. What it does is that it stores these pairs at a certain index using a function, this way it has an O time of 1, which is optimal when wanting to get the value from an array that is big.

The formula of hashing involved adding up the ACII values of they key, multiplying them by a prime number like 5 and then getting the modulo, and that is your index.

Collisions are what happens when two pairs are stores at the same index, since the placement depends on the key.
