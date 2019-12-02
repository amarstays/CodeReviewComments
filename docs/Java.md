# Java

Some of the checks are common across programming languages.

Checklist Item | Category
-------------- | --------
Classes should be small. Defined the number based on the domain | Classes
Always override hashCode when you override equals | Classes
Always override toString for Classes in model | Classes
Make class final if not being used for inheritance | Classes
Minimize the accessibility of Packages, Classes and Members | Classes and Interfaces
In public classes, use accessor methods, not public fields | Classes and Interfaces
Functions should be small! | Methods
Do one Thing | Methods
Check parameters for validity | Methods
Return empty arrays or collections, not nulls | Methods
Don't Repeat Yourself (Avoid Duplication) | Methods
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
Explain yourself in code | Comments
Document thread safety | Comments
Use Exceptions rather than Return codes | Exceptions
Use checked exceptions for recoverable conditions and runtime exceptions for programming errors | Exceptions
Favor the use of Java standard(defined) exceptions | Exceptions
Don't ignore exceptions (At least log a debug message) | Exceptions
Any use of the SecurityManager highlights an area that should be scrutinized | Security
Establish trust boundaries between caller and called by validations | Security
Beware of activities that may use disproportionate resources | Security
Purge sensitive information from exceptions and logs | Security
Consider purging highly sensitive from memory after use without waiting for GC | Security
Do not try to correct input data. Reject | Security
Take care interpreting untrusted code `i.e. javax.script` | Security
Prevent injection of exceptional floating point values | Security
Limit exposure of `ClassLoader` instances and impose access control on `ClassLoader` | Security
Avoid serialization for security-sensitive classes | Security
Be careful caching results of potentially privileged operations or data | Security
Defensive use of the Java Native Interface (JNI) | Security
Minimize the scope of local variables | General Programming
Refer to objects by their interfaces | General Programming
Adhere to generally accepted naming conventions | Meaningful Names
Use Intention-Revealing Names | Meaningful Names
Pick one word per concept | Meaningful Names
Use Solution/Problem Domain Names | Meaningful Names

## Reference

Code Complete - Steve McConnell
[Oracle Guide](https://www.oracle.com/technetwork/java/seccodeguide-139067.html) - More details about most of the above can be found here.
