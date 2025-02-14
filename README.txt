COMP 313/413 Project 2 Report

TestList.java and TestIterator.java

	Try with a LinkedList - does it make any difference?

		It does not make a difference.

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			Removes the element at index 5

		list.remove(Integer.valueOf(5)); // what does this one do?

			Removes the first instance of 5 in the list

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			It would only remove the first instance of 77 in the list

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
				  #1     #2     #3
        testArrayListAddRemove:  351ms  314ms  240ms
        testLinkedListAddRemove:  20ms   19ms   21ms
	testArrayListAccess:      11ms   11ms   12ms
        testLinkedListAccess:     11ms    9ms    9ms

	SIZE 100
				  #1     #2     #3
        testArrayListAddRemove:  323ms  385ms  358ms
        testLinkedListAddRemove:  18ms   19ms   20ms
	testArrayListAccess:      14ms   11ms   12ms
        testLinkedListAccess:     20ms   21ms   23ms

	SIZE 1000
				  #1     #2     #3
        testArrayListAddRemove:  419ms  469ms  485ms
        testLinkedListAddRemove:  18ms   19ms   20ms
	testArrayListAccess:      10ms   11ms   11ms
        testLinkedListAccess:    205ms  328ms  328ms

	SIZE 10000
				     #1            #2              #3
        testArrayListAddRemove:   2sec 96ms     1sec 896ms      1sec 779ms
        testLinkedListAddRemove:       22ms           22ms            23ms
	testArrayListAccess:           13ms           12ms            13ms
        testLinkedListAccess:    4sec 730ms     4sec 661ms      4sec 211ms

	listAccess - which type of List is better to use, and why?

		ArrayList: Constant time access to elements (O(1))

	listAddRemove - which type of List is better to use, and why?

		LinkedList: Constant time to insert or delete elements (O(1))
