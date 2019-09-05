Collective Ownership
 
 Collective Ownership encourages everyone to contribute new ideas to all segments of the project. Any developer can change any line of code to add functionality, fix bugs, improve designs or refactor. No one person becomes a bottle neck for changes.
 This is hard to understand at first. It's almost inconceivable that an entire team can be responsible for the system's design. Not having a single chief architect that keeps some visionary flame alive seems like it couldn't possibly work.
 But it is not uncommon to ask a chief architect a question and get an answer that is just plain wrong. It is not a failing of your lead programmers. Any non-trivial system can not be held in one person's mind. Other programmers are hard at work changing the system without benefit of the architect's vision. Whether you realize it or not your design is already distributed among your team. If the entire team already has some responsibility for design decisions, shouldn't they receive the authority as well?
 The way this works is for each developer to create unit tests for their code as it is developed. All code that is released into the source code repository includes unit tests that run at 100%. Code that is added, bugs as they are fixed, and old functionality as it is changed will  be	
covered by automated testing. Now you can rely on the test suite to watch dog your entire code repository. Before any code is released it must pass the entire test suite at 100%.
 Once this is in place anyone can make a change to any method of any class and release it to the code repository as needed. When combined with frequent integration developers rarely even notice a class has been extended or repaired.
 In practice collective ownership is actually more reliable than putting a single person in charge of watching specific classes. Especially since a person may leave the project at any time. Optimize Last

Portland Pattern RepositoryXProgramming.com
