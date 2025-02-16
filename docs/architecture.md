

#### [SOLID principles](https://x.com/NikkiSiapno/status/1890986211633959413)
- S — Single Responsibility Principle
- O — Open/Closed Principle
- L — Liskov Substitution Principle
- I — Interface Segregation Principle
- D — Dependency Inversion Principle

Let’s break down each principle

1. **Single Responsibility Principle (SRP):** Each unit of code should only have one job or responsibility. A unit can be a class, module, function, or component. This keeps code modular and removes the risk of tight coupling.
2. **Open-Closed Principle (OCP):** Units of code should be open for extension but closed for modification. You should be able to extend functionality with additional code rather than modifying existing ones. This principle can be applied to component-based systems such as a React frontend.
3. **Liskov Substitution Principle (LSP):** You should be able to substitute objects of a base class with objects of its subclass without altering the ‘correctness’ of the program. An example of this is with a Bird base class. You might assume that it should have a ‘fly’ method. But what about the birds that can’t fly? Like a Penguin. In this example, having a ‘fly’ method in the Bird class would violate LSP.
4. **Interface Segregation Principle (ISP):** Provide multiple interfaces with specific responsibilities rather than a small set of general-purpose interfaces. Clients shouldn’t need to know about the methods & properties that don't relate to their use case.
    - Complexity ↓
    - Code flexibility ↑
5. **Dependency Inversion Principle (DIP):** You should depend on abstractions, not on concrete classes. Use abstractions to decouple dependencies between different parts of the systems. Direct calls between units of code shouldn’t be done, instead interfaces or abstractions should be used.

    ![image](https://github.com/user-attachments/assets/284b377a-3ee0-425b-adf4-baa708fea65a)

These principles gives a lens into the foundations of clean code which can be applied to many areas of programming.
