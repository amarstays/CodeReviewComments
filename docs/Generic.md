# Generic

Some of the General Programming, Naming, Comment, Error Handling, Security, Design checks are common across programming languages.

Checklist Item | Category
-------------- | --------
Explain yourself in code | Comments
Don't ignore exceptions (At least log a debug message) | Error Handling
Purge sensitive information from exceptions and logs | Security
Consider purging highly sensitive data from memory after use. | Security
Do not try to correct input data. Reject the request | Security
Be careful caching results of potentially privileged operations or data | Security
Functions / Methods should be small! | General Programming
Do one Thing | General Programming
Check parameters for validity | General Programming
Minimize the scope of local variables | General Programming
Use appropriate logger | General Programming
Don't Repeat Yourself (Avoid Duplication) | General Programming
Use appropriate language / framework scaffolding | General Programming
Use appropriate package manager / build for dependencies | General Programming
Adhere to generally accepted naming conventions | Meaningful Names
Use Intention-Revealing Names | Meaningful Names
Pick one word per concept | Meaningful Names
Use Solution/Problem Domain Names | Meaningful Names
Always use a logger service when application runs on cloud | Design
Prefer immutability for value types | Design
Configs are separated from the code | Design
