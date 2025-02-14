Try with a LinkedList - does it make any difference?
    It does not make a difference
What happens if you use list.remove(Integer.valueOf(77))?
    It would only remove the first instance of 77 in the list
Try with a LinkedList - does it make any difference?
    It does not make a difference
What does this method do?
    Removes the element at index 5
What does this one do?
    Removes the first instance of 5 in the list
Run test and record running times for SIZE = 10, 100, 1000, 10000, ...
    testArrayListAccess: 10 - 10ms, 100 - 10ms, 1000 - 12ms, 10000 - 13ms
    testLinkedListAccess: 10 - 9ms, 100 - 21ms, 1000 - 328ms, 10000 - 4sec 547ms
    testArrayListAddRemove:10 - 356ms, 100 - 359ms, 1000 - 489ms, 10000 - 2sec 99ms
    testLinkedListAddRemove:10 - 20ms, 100 - 19ms, 1000 - 20ms, 10000 - 22ms
What conclusions can you draw about the performance of LinkedList vs. ArrayList when comparing their running times for AddRemove vs. Access?
    Access:
        LinkedList: Access times grow dramatically with size
        ArrayList: Maintains fast access times as size grows
    AddRemove:
        LinkedList: Maintains fast AddRemove times as size grows
        ArrayList: AddRemove times grow dramatically with size
    Conclusion:
        LinkedList excels at AddRemove while ArrayList does not
        ArrayList excels at Access while LinkedList does not
