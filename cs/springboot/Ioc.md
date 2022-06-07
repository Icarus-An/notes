
# IoC Container

The containder will create the objects, wire them together, configure them, and manage their complete life cycle from creation till destruction.

## IoC - Inversion of Control

Implemented by dependency injection.
Separate the creation and configuration of components from the use of components.
Instead of instantiate a component manually, we let the spring container to create and config the component singleton and pass it to other component. Then let the spring container to manage the lifecycle of the component.

### Dependency Injection
Implemented by setter method or constructor with parameter or field injection().
- Setter method injection is recommended to use on Optional dependencies, the dependency can be changed after the object is instantiated.
- Constructor injection is recommended to use on Mandatory dependencies, since the dependency is ready for using once the object has been instantiated.
- Field injection is not recommended but most used because it's very easy 
    - it could cause cicular dependency problem A depends on B and B depends on A.
    - it will increase the coupling between classes and containers, the class cannot be used without container. Which is not good for testing and so on.
Pass the component instance into the program instead of creating the component manually

