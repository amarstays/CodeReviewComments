# Unit Tests

## Checklist Items

1. Test class is testing only one class.
2. Test case is testing only one method / unit.
3. One method could have more than one test.
4. Tests has intention revealing names.
5. Given same care naming the test variables as product code. A special attention is paid when naming test variables. I.e. inputDateFoo_Past expectFoo_PastDate
6. Test code is clean as the product code.
7. Avoid using condition in the test case. A condition means multiple test cases.
8. Avoid any calls to external services from the test. I.e. Calling a database.
9. Developers can use mocks to simulate functionality which is not available at the beginning of writing the product code. But do not use mocks to simulate external I/O bound services. I.e. Databases, Email Services etc... If mocks are used in tests which has business logic this means the code needs some redesign. I.e. Dependency Inversion.
10. Tests should focus on testing business requirements. Business requirement could be implemented using pure functions without any side effects by separating the state out from the business requirement. Write the unit test for the business requirement pure function not to the impure state holding function.
11. Test should not consider any side effects from the code under test for assertions. I.e. The test code's input parameters should not be used to assert the result of the test. This is not a problem of the test but a problem in the code. I.e. Mutation of the input
12. Test code input values should be static. Avoid changes to input value is changing based on the context or time it runs
13. Input values of a test should be representative of the real inputs. I.e. fullName='Peter Pan' not fullName='TestTest'.
14. Test do not need any manual handling prior to execution.
15. A test suite should not have any ignored /commented test cases.
16. Avoid using delays or sleep in the test.
17. Test suite should be super fast.
