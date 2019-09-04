# 测试先行

如果你在编写产品代码前先编写测试，你会觉得创建产品代码更加容易和快速了。相比直接实现产品代码，先编写单元测试与使之通过的产品代码所需的时间相差无几，但有了单元测试在手，你省去了先写产品代码时需要后补测试的时间，也为以后省下了许多时间。

> When you create your tests first, before the code, you will find it much easier and faster to create your code. The combined time it takes to create a unit test and create some code to make it pass is about the same as just coding it up straight away. But, if you already have the unit tests you don't need to create them after the code saving you some time now and lots later.

编写单元测试能促使开发者思考真正需要开发的东西。于是，需求会被扎实地分解成一个个测试，透过可执行代码这种形式固定下来，任何人都可以准确地理解它们。

> Creating a unit test helps a developer to really consider what needs to be done. Requirements are nailed down firmly by tests. There can be no misunderstanding a specification written in the form of executable code.
 
测试可以在编码时给你即时的反馈。通常，我们不容易知道开发者是否真的完成了所有的功能，因为需求范围可能悄悄扩张，可能新增了一些错误条件的处理。如果我们确实通过测试先行的方式工作，那就可以清楚地知道工作是否完成：只需要看是否所有单元测试都通过即可。
 
> You also have immediate feedback while you work. It is often not clear when a developer has finished all the necessary functionality. Scope creep can occur as extensions and error conditions are considered. If we create our unit tests first then we know when we are done; the unit tests all run.
 
 此外，测试先行对系统设计也有所裨益。一些软件系统是通过先实现后测试的顺序构建——并且测试往往由另一个全然不同的团队负责——你很难对这样的系统进行单元测试。通过测试先行的方式，所有具备用户价值的代码都需要被测试，这种动力将反过来影响系统的设计。系统将因此留下测试的刻痕，那就是它们都非常容易被测试。
 
 > There is also a benefit to system design. It is often very difficult to unit test some software systems. These systems are typically built code first and testing second, often by a different team entirely. By creating tests first your design will be influenced by a desire to test everything of value to your customer. Your design will reflect this by being easier to test.
 
 这种先写测试的软件开发方式是有节奏的。你会先写一个测试，描述手上要解决的一个小问题，然后编写最简单的代码使测试通过。接着再编写第二个测试，然后在刚刚实现的代码上再次编写代码，使测试通过。但是注意不要过度实现！请通过新的测试来驱动实现。你应该重复这个过程，一直到所有需求全部变成测试用例为止。coffee maker完整地展示了这个过程，它是一个用Java写成的例子。
 
 > There is a rhythm to developing software unit test first. You create one test to define some small aspect of the problem at hand. Then you create the simplest code that will make that test pass. Then you create a second test. Now you add to the code you just created to make this new test pass, but no more! Not until you have yet a third test. You continue until there is nothing left to test. The coffee maker problem shows an example written in Java.

测试驱动出来的代码都十分简洁，只会实现你需要的功能。其他开发者可以通过浏览测试了解代码的用法。??
 
> The code you will create is simple and concise, implementing only the features you wanted. Other developers can see how to use this new code by browsing the tests. Input whose results are undefined will be conspicuously absent from the test suite. 
