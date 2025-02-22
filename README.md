Online Shopping System

This Java project demonstrates the implementation of the five SOLID principles through an Online Shopping System. The system enables users to place and cancel product orders while offering various payment methods and delivery options. Each component is designed to align with one of the SOLID principles to ensure the code is clean, maintainable, and scalable.

The Single Responsibility Principle is applied through the Product class, which focuses solely on representing product data such as ID, name, and price. This ensures that the class has only one reason to change. The Open/Closed Principle is addressed with the PaymentStrategy interface and its implementations like CreditCardPayment and PayPalPayment. This design allows the system to support new payment methods without altering existing code, making it extensible yet stable.

The Liskov Substitution Principle is demonstrated through the Delivery abstract class and its subclasses, HomeDelivery and StorePickup. These classes ensure that any subclass can replace the base class without affecting the overall functionality. The Interface Segregation Principle is reflected in the OrderOperations interface, which provides only the necessary methods for order placement and cancellation. This prevents classes from being forced to implement methods they do not need.

The Dependency Inversion Principle is applied by ensuring high-level modules such as the Order class depend on abstractions like PaymentStrategy and Delivery rather than concrete implementations. This approach enhances flexibility and reduces coupling between components.

The OnlineShoppingSystem class contains the main method, showcasing how products are created, payment methods and delivery options are selected, and orders are processed. The overall design promotes code reusability and scalability while requiring minimal changes when extending or modifying features.
