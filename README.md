# Professor Ranking

Awarded third Place at UTEC-Introduction to Computer Science Project Fair.

3. Ranking of professors.
- Given a list of professors, create the functionality to search for teachers by their first name, by a part of their name, by their last name.
- Choose a teacher and rate him by the following criteria:
- Communication level in the classroom (1-10)
- Exam level (1-10)
- Assistance Control (yes/no)
- Didactic level (1-10)
- Easy or Demanding.

What makes this project interesting is its implementation: we tried to emulate an early sketch of Google's Search Engine. A Binary Search Tree (BST), in which each node represented a letter of the alphabet, was implemented. Afterwards, for each node we added a Trie starting with that letter (informally, this is a "BST of Tries"), so that the Professor names would be stored in these Tries. 

It can be proven that the estimated time complexity for each query is approximately O(1) after having memoized enough examples. This is really a development over the trivial algorithm, which would compare all letters of the string and find the maximum match after a complete search (these operations can be up to O(length of the string * number of names in the databes * average length of stored names). 
