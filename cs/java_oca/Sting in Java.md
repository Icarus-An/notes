# String in Java

## String, String Buffer, String Builder

### String

String is stored as a final char array, so once it is been created, it cannot be changed.

    private final char value[]    

Stack, Heap, String Table (in Heap)

    Stack will store the reference of the String.
    String object will be created in Heap when explicit invoke the string constructor.
    String Table will be created in the Heap during compling. It is used to store String object.

String in double quote

    Usually we create string like String str = "abc", the double quote string will be created and stored in String Table for reuse.



