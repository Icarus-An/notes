# Grabage Collection	
    
    Java garbage collection is an automatic process. 
	Automatic garbage collection is the process of looking at heap memory, identifying which objects are in use and which are not, and deleting the unused objects. 
	An in-use object, or a referenced object, means that some part of your program still maintains a pointer to that object. An unused or unreferenced object is no longer referenced by any part of your program. 
	So the memory used by an unreferenced object can be reclaimed. The programmer does not need to mark objects to be deleted explicitly. The garbage collection implementation lives in the JVM. 
	- There are generally four ways to make an object eligible for garbage collection.
	1. Nullifying the reference variable
	2. Re-assigning the reference variable
	3. An object created inside the method
	4. Island of Isolation
