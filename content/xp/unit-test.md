<!-- # Unit Tests

Unit tests are one of the corner stones of Extreme Programming (XP). But unit tests XP style is a little different. First you should create or download a unit test framework to be able to create automated unit tests suites. Second you should test all classes in the system. Trivial getter and setter methods are usually omitted. You will also create your tests first, before the code.

Unit tests are released into the code repository along with the code they test. Code without tests may not be released. If a unit test is discovered to be missing it must be created at that time.

The biggest resistance to dedicating this amount of time to unit tests is a fast approaching deadline. But during the life of a project an automated test can save you a hundred times the cost to create it by finding and guarding against bugs. The harder the test is to write the more you need it because the greater your savings will be. Automated unit tests offer a pay back far greater than the cost of creation.

Another common misconception is that unit tests can be written in the last three months of  the project. Unfortunately, without the unit tests development drags on and eats up those last three months and then some. Even if the time is available good unit test suites take time to evolve. Discovering all the problems that can occur takes time. In order to have a complete unit test suite when you need it you must begin creating the tests today when you don't.

Unit tests enable collective ownership. When you create unit tests you guard your functionality from being accidentally harmed. Requiring all code to pass all unit tests before it can be released ensures all functionality always works. Individual code ownership is not required if all classes are guarded by unit tests.

Unit tests enable refactoring as well. After each small change the unit tests can verify that a change in structure did not introduce a change in functionality.

Building a single universal unit test suite for validation and regression testing enables frequent integration. It is possible to integrate any recent changes quickly then run your own latest version of the test suite. When a test fails your latest versions are incompatible with the team's latest versions. Fixing small problems every few hours takes less time than fixing huge problems just before the deadline. With automated unit tests it is possible to merge a set of changes with the latest released version and release in a short time.

Often adding new functionality will require changing the unit tests to reflect the functionality. 

While it is possible to introduce a bug in both the code and test it rarely happens in actual practice. It does occasionally happen that the test is wrong, but the code is right. This is revealed when the problem is investigated and is fixed. Creating tests independent of code, hopefully before code, sets up checks and balances and greatly improves the chances of getting it right the first time.

Unit Tests provide a safety net of regression tests and validation tests so that you can refactor and integrate effectively. As they say at the circus; never work without a net! Creating the unit test before the code helps even further by solidifying the requirements, improving developer focus, and avoid creeping elegance.

-->

# 单元测试

单元测试是极限编程（XP）的基石之一。但是XP风格的单元测试又有点儿不同。首先，你应该创建或下载一个单元测试框架，以便能够创建自动化的单元测试套件。其次，你应该测试系统中的所有类。通常省略一些简单的getter和setter方法。你还必须在写代码之前先写测试。

单元测试与它们测试的代码一起发布到代码存储库中。未经测试的代码不能被发布。如果发现某个单元测试缺失，则必须马上创建它。

投入大量时间在单元测试上的最大阻力通常是“项目快到最后期限了”。但是在项目的生命周期中，自动化测试通过发现和防范错误，可以为你节省百倍的时间和成本。测试越难写，你就越需要它，因为你节省的时间成本就越多。自动化单元测试所提供的回报远远大于创建它的成本。

另一个常见的误区是，单元测试可以在项目的最后三个月内编写。不幸的是，没有单元测试的开发会拖延并消耗掉那三个月甚至更多的时间。即使时间允许，也还是需要很多时间来形成好的单元测试套件，因为发现所有可能发生的问题需要很多时间。为了在需要时拥有一个完整的单元测试套件，我们必须从一开始（也许并不需要的时候）就创建测试。

单元测试支持集体所有权。当你创建单元测试时，你可以保护你的功能不受意外伤害。要求所有代码在发布之前通过所有单元测试，确保所有功能始终正常工作。如果所有类都由单元测试保护，则不需要单独的代码所有权。

单元测试也支持重构。在每一个小的变更之后，单元测试都可以确保结构上的变更不会引起功能上的变更。

为验证和回归测试构建一个通用的单元测试套件可以很好地支持持续集成。它可以快速集成任何最近的更改，然后运行你最新版本的测试套件。当测试失败时，说明你的最新版本与团队的最新版本不兼容。每隔几个小时解决一个小问题比在最后期限前解决一个大问题要花更少的时间。通过自动化单元测试，可以很快地将一组更改与最新版本的代码合并，并发布。

通常添加新功能需要更改单元测试以反映功能需求。

虽然在代码和测试中同时引入错误是有可能的，但在实际情况中却很少发生。确实会发生单元测试错误，但代码是正确的情况。通常研究一个问题并把它解决之后才会暴露出来。创建独立于代码的测试，当然最好是在写代码之前，可以建立**检查和制约**<sup>[注1](#checks_balances)</sup>，并大大提高从一开始就做对的机会。

单元测试提供了回归测试和验证测试的安全网，以便你可以有效地重构和集成。就像马戏团里常说的：没有网就不要工作！在代码之前创建单元测试有助于进一步确定需求，提高开发人员的专注度，并避免过度设计。

<a name="checks_balances">注1</a> 检查和制约：是指因为在写代码之前先写了测试，而在写代码时则要且仅要保证测试运行通过。这样代码就受到了检查和制约，也就是说保证了即不出现功能错误也不过度设计，提高了从一开始就向正确的方向演进的机会。
: Footnote content goes here