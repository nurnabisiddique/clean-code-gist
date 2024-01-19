# clean-code-gist
Clean Code Gist summary by robert c martin

|| Summary of 'Clean code' by Robert C. Martin ||

Code is clean if it can be understood easily by everyone on the team and enhanced by a developer other than its original author with understandability, changeability, extensibility and maintainability.

General rules
- Keep it simple stupid. Simpler is always better. Reduce complexity as much as possible.
- Boy scout rule. Leave the campground cleaner than you found it.
- Always find root cause. Always look for the root cause of a problem.

Comments rules
- Always try to explain yourself in code.
- Don't be redundant.
- Don't add obvious noise.
- Don't use closing brace comments.
- Don't comment out code. Just remove.
- Use as explanation of intent.
- Use as clarification of code.
- Use as warning of consequences.

Design rules
- Keep configurable data at high levels.
- Prefer polymorphism to if/else or switch/case.
- Separate multi-threading code.
- Prevent over-configurability.
- Use dependency injection.
- Follow Law of Demeter. A class should know only its direct dependencies.

Source Code Structure
- Separate concepts vertically.
- Related code should appear vertically dense.
- Dependent functions should be close.
- Similar functions should be close.
- Place functions in the downward direction.
- Prefer fewer arguments.
- Keep lines short.
- Don't use horizontal alignment.
- Don't use flag arguments. Split method into several independent methods that can be called from the client without the flag.
- Don't break indentation.

Objects and data structures
- Hide internal structure.
- Proper data structures.
- Avoid hybrids structures (half object and half data).
- Should be small.
- Do one thing.
- Small number of instance variables.
- Base class should know nothing about their derivatives.
- Better to have many functions than to pass some code into a function to select a behavior.

Understandability tips
- Be consistent. If you do something a certain way, do all similar things in the same way.
- Encapsulate boundary conditions. Boundary conditions are hard to keep track of. Put the processing for them in one place.
- Prefer dedicated value objects to primitive type.
- Avoid logical dependency. Don't write methods which works correctly depending on something else in the same class.
- Avoid negative conditionals.

Naming rules
- Choose descriptive and unambiguous names.
- Use pronounceable names.
- Use searchable names.
- Replace magic numbers with named constants.
- Avoid encodings.

Tests
- One assert per test.
- Readable.
- Fast.
- Independent.
- Repeatable.

Avoid code smells
- Rigidity. The software is difficult to change. A small change causes a cascade of subsequent changes.
- Fragility. The software breaks in many places due to a single change.
- Immobility. You cannot reuse parts of the code in other projects because of involved risks and high effort.
- Needless Complexity.
- Needless Repetition.
- Opacity. The code is hard to understand.

