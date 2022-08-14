## Design Principles

###  [**SOLID**](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design) - The First 5 Principles of Object Oriented Design
> ***SRP*** (Single Responsibility Principle)
> + `suggests that a class should have only one reason to change`
> + `divide into summing part and output part`

> ***OCP*** (Open-Closed Principle)
> + `states Objects or entities should be open for extension but closed for modification`
> + `create interface and use `implements`  keyword  to create various types of subclasses `

> ***LSP*** (Liskov Substitution Principle)
> + `let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a subtype of T.`

> ***ISP*** (Interface Segregation Principle)
> + `A client should never be forced to implement an interface that it doesn't use, or clients shouldn't be forced to depend on methods they do not use`

> ***DIP*** (Dependency Inversion Principle)
> + `entities must depend on abstactions, not on concretions.`
> + `high-level module must not depend on the low-level module, but they should depend on abstractions.`
