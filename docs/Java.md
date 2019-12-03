# Java

Checklist Item | Category
-------------- | --------
Classes should be small. Defined the number based on the domain | Classes
Always override hashCode when you override equals | Classes
Always override toString for Classes in model | Classes
Make class final if not being used for inheritance | Classes
Minimize the accessibility of Packages, Classes and Members | Classes and Interfaces
In public classes, use accessor methods, not public fields | Classes and Interfaces
Return empty arrays or collections, not nulls | Methods
Create safe copies of mutable and subclass-able input values in side methods before work on them | Methods
Create copies of mutable output values before return | Methods
Treat passing input to `untrusted object` as output (pass a copy) | Methods
Treat output from `untrusted object` as input (work on copy of returned) | Methods
Make public static fields final | Constants and Variables
Appropriate use of deep and shallow coping of objects | Design
Prefer Composition over Inheritance. If inheritance is used make sure to apply LISKOV substitution principle | Design
Prefer immutability for value types | Design
Beware of excessive Object creation (i.e. String objects) due to garbage and concurrency | Object Construction
Avoid exposing constructors of sensitive classes. Use static factory method | Object Construction
Defend against cloning of non-final classes | Object Construction
View deserialization the same as object construction | Object Construction
Use enums instead of int constants | Enums and Annotations
Use marker interfaces to define types | Enums and Annotations
Document thread safety | Comments
Use Exceptions rather than Return codes | Error Handling
Use checked exceptions for recoverable conditions and runtime exceptions for programming errors | Error Handling
Favor the use of Java standard(defined) exceptions | Error Handling
Any use of the SecurityManager highlights an area that should be scrutinized | Security
Establish trust boundaries between caller and called by validations | Security
Beware of activities that may use disproportionate resources | Security
Consider purging highly sensitive data from memory after use without waiting for GC | Security
Take care interpreting untrusted code `i.e. javax.script` | Security
Prevent injection of exceptional floating point values | Security
Limit exposure of `ClassLoader` instances and impose access control on `ClassLoader` | Security
Avoid serialization for security-sensitive classes | Security
Defensive use of the Java Native Interface (JNI) | Security
Refer to objects by their interfaces | General Programming

## Reference

* Code Complete - Steve McConnell
* [Oracle Guide](https://www.oracle.com/technetwork/java/seccodeguide-139067.html) - More details about most of the above can be found here.
