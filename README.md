# Maintainable Software Guidelines

1. **Keep functions, methods, and constructors concise.**
    - Try to restrict functions to a maximum of 15 lines.
    - Use object initializers and functional decomposition to simplify complex functions.
  
2. **Minimize decision points in your code.**
    - Limit branching to a maximum of four times per function/method.
    - Leverage Object-Oriented Programming (OOP) principles to simplify decision points.
    - If a code block can be described with a comment, it's usually a good candidate to be turned into a function.

3. **Avoid code duplication.**
    - Code should be written once and reused where necessary to maintain consistency and reduce errors.

4. **Keep the size of method parameters and constructors manageable.**
    - Parameters that are frequently used together can be encapsulated in their own object.

5. **Separate concerns into different modules or classes.**
    - Strive for modularity to ensure each part of your software has a single responsibility.
    - Avoid large modules that are difficult to manage and understand.
    - Hide implementation details behind interfaces.

6. **Top-level components should be loosely coupled.**
    - Minimize the amount of code in one module that interacts with code in another module.
    - Try to limit the number of entry points from one component to another.
    - Make use of patterns like Abstract Factory to manage dependencies effectively.
    - Refactor "Manager" classes or high-traffic service calls to reduce complexity.

7. **Balance architecture components.**
    - Aim for around 9 top-level components, with a range between 6 and 12.
    - The structure of top-level components should reflect the structure of lower-level components.

8. **Maintain a lean codebase.**
    - Regularly refactor and clean up your code to prevent unnecessary bloat.
    - Smaller codebases are easier to manage, understand, and test.

9. **Automate your development pipeline and tests.**
    - Convert manual tests into automated ones where possible.
    - Maintain a robust suite of unit tests.
    - The length of your unit tests should be around 80% of your total codebase.
    - Writing unit tests encourages the development of maintainable code.

10. **Ensure code cleanliness.**
    - Remove or refactor code that generates warnings or has code smells.
    - Keep comments accurate and meaningful; remove unnecessary ones.
    - Remove commented-out code blocks.
    - Eliminate dead code (code that is never executed).
    - Use clear, descriptive names for identifiers.
    - Replace magic numbers with named constants.
    - Handle exceptions properly; don't leave any uncaught exceptions.
