Recently we've received a requirement to create a basic banking system.

These are the requirements for the system:
  - Create accounts (you need a positive initial balance to open an account)
  - List accounts (with all properties)
  - Receive deposits
  - Accept withdraws
    
Account properties:
  - Account number
  - First and Last name owner
  - Balance

The project needs to be developed using WebApi. You can use any library / NuGet package in the solution through a REST API.
There is no an correct answer for the project so show us what you can do.

If you think that you cannot complete the solution but you can explain the missing parts in plain text its ok too.

Bonus points:
  - Logging
  - Audit

---------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------

Answer: There is no a correct answer, I try to get an idea about how the candidate can resolve it applying all concepts as much he can.

Possible architectures:
  - Controller / Service / Repository
    - Dependency injection
    - Validation
    - Logging

  - Event Sourcing
    - Dependency injection
    - Validation
    - Logging
    - Audit is implicit in the architecture because we're saving the events and no the current state

Points to review in the solution:
  - REST
  - Design patterns
  - Dependency injection
  - Validation (account not found, no withdraw with insufficient funds)
  - How the balance is calculated (save every transaction vs update the account number balance)
