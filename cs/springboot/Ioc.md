
# IoC Container

The containder will create the objects, wire them together, configure them, and manage their complete life cycle from creation till destruction.

## IoC - Inversion of Control

Implemented by dependency injection.
Separate the creation and configuration of components from the use of components.
Instead of instantiate a component manually, we let the spring container to create and config the component singleton and pass it to other component. Then let the spring container to manage the lifecycle of the component.

### Dependency Injection
Implemented by set() method or constructor with parameter.
Pass the component instance into the program instead of creating the component manually

