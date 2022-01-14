- # Class Declatations and Modifiers 
  - ## Final Classes  
    - The final keyword means the class can't be subclassed. In practice, you'll almost never make a final class.  
    - You should make a final class only if you need an absolute guarantee that none of the methods in that class will ever be overridden
  - ## Abstract Classes  
    - An abstract class can never be instantiated.  
    - *Notice that the methods marked abstract end in a semicolon rather than curly braces.  
    - The first concrete subclass of an abstract class must implement all abstract methods of the suoperclass.  
  - ## Difference between protected and default (none) Modifier  
    1. ### Two way of accessing member: Inheritance and Reference  
       inheritance: (access by subclass), reference: (access by dot "." operator), same package, outside package.  
    2. ### Protected modifier  
       Only cannot access from outside package by inheritance.  
       Once the subclass-outside-the-package inherits the protected member, that member (as inherited
by the subclass) becomes private to any code outside the subclass, with the exception of subclasses of the
subclass.
    3. ### default (none) modifier  
       Can only access from same package
