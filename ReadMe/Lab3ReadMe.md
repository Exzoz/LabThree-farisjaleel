TestIterator Questions 

TODO also try with a LinkedList - does it make any difference?

      - As far as the test results it has no effect on the results when testing

2)  TODO what happens if you use list.remove(Integer.valueOf(77))?

     - Doing this would throw java.util.ConcurrentModificationException. Essentially this means that something was changed was transferring over using an iterator. It is very common when using collections. 

TestList Questions

1)   TODO also try with a LinkedList - does it make any difference?

      - As far as the test results it has no effect on the results when testing

2)   list.remove(5); // what does this method do?

      - In this method, we are removing the element at this specific position in the list. So position 5 would be for element 77. 

3) list.remove(Integer.valueOf(5)); // what does this one do?

    - In this method we are removing the first occurrence of the specific element, which is 5 in this case, from the list. 

TestPerformance Questions + Results

Size : 10, Reps: 100000000
testArrayListAccess              0.286s
testLinkedListAddRemove.   0.884s
testLinkedListAccess            0.474s
testArrayListAddRemove.     1.905s

Size : 100, Reps: 10000000
testArrayListAccess              0.289s
testLinkedListAddRemove.   0.785s
testLinkedListAccess            1.805s
testArrayListAddRemove.     4.472s

Size : 1000, Reps: 10000000
testArrayListAccess              0.326s
testLinkedListAddRemove.   0.793s
testLinkedListAccess            35.227s
testArrayListAddRemove.     28.143s

  // which of the two lists performs better as the size increases?
 
        - For the add or remove operations, LinkedList had better performance results compared to ArrayList. As far as Access, ArrayList had better performance than LinkedList. 





> Written with [StackEdit](https://stackedit.io/).