# String in Java

https://mp.weixin.qq.com/s/f6VTVXktADP7U1BmlUWM-Q
https://cloud.tencent.com/developer/article/1686226

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


### StringBuffer and StringBuilder

StringBuffer and StringBuilder are both extend from AbstractStringBuilder，their length is variable.

    char[] value;

StringBuilder is faster than StringBuffer, cause StringBuffer used "synchronized" keyword to guarantee thread safey, which causes a performance loss.


new String("abc");
创建了一个或两个对象，一定会在堆中创建一个对象， "abc"可能已经存在于字符串常量池中。

String str = "abc" + "def";
创建一个对象，使用＋拼接双引号字符串，在编译期间会被直接优化成 "abcdef"

String str = "abc" + new String("def");
创建了4个字符串对象和1个StringBuilder对象。