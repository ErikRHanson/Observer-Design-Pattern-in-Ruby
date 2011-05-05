# Design Patterns in Ruby: Observer Pattern

This is the observer pattern from [*Design Patterns in Ruby*](http://www.designpatternsinruby.com/) by [Russ Olsen]

ex1/employee.rb contains the first attempt at creating two classes, Employee and Payroll in wich the employee class calls the update method of the Payroll class d
directly.  The implementation is troublesome because it relies on a high degree of coupling between the two classes.


observer1/employee.rb contains the first attempt to implement the Observer pattern.  This time the 
Employee object contains an array of observers which we can use to keep track of anything which may 
want to to keep watch on our Employee.  To keep things names properly, the GoF would now consider 
our employee class to be the **subject** and the Payroll, TaxMan, and any other class we add into the 
observers array, to be the **observers**.

observer2/  **something went wrong **

observer3/sub_mod.rb  implements the Observer Patterin using a Ruby module to mix-in the observer functionality

observer4/rby_observer.rb uses Ruby\'s built in 'observer' class to implement the observer pattern in a very "Ruby" way.

observer5/observer.rb users a code block to pass a code block for each observer into the subject.
