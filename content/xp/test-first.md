# 测试先行

如果你在编写产品代码前先编写测试，你会发现编写产品代码更加容易、更加快速了。相比于直接上手实现代码，先编写[单元测试](unit-test.md)、再编写使之通过的产品代码，所需的时间相差无几。但有了单元测试在手，你就节省了先写产品代码时需要后补测试的时间，并为日后的排错省下了更多时间。

<!-- When you create your tests first, before the code, you will find it much easier and faster to create your code. The combined time it takes to create a unit test and create some code to make it pass is about the same as just coding it up straight away. But, if you already have the unit tests you don't need to create them after the code saving you some time now and lots later. -->

编写单元测试能促使开发者思考，什么是真正需要开发的东西。他们会将需求扎实地分解成一个个测试，透过可执行的测试代码这种形式固定下来。这样记录下来的需求没有任何误解的空间。

<!-- Creating a unit test helps a developer to really consider what needs to be done. Requirements are nailed down firmly by tests. There can be no misunderstanding a specification written in the form of executable code. -->

测试可以在编码时给你即时的反馈。通常而言，我们不容易知道开发者是否真的完成了所有的功能，因为需求范围可能悄悄扩张，可能新增了一些错误条件的处理。如果用测试先行的方式工作，那就可以清楚地知道工作何时完成：只需要看是否所有单元测试都通过即可。

<!-- You also have immediate feedback while you work. It is often not clear when a developer has finished all the necessary functionality. Scope creep can occur as extensions and error conditions are considered. If we create our unit tests first then we know when we are done; the unit tests all run. -->
 
此外，测试先行对系统设计也有所裨益。很多软件系统是以“先实现、后测试”的次序构建的，而且测试往往由另一个全然不同的团队负责。对这样的系统进行单元测试往往困难重重。通过测试先行的方式，所有具备用户价值的代码都需要被测试，这种动力将反过来影响系统的设计。你的设计将很容易被测试——这正是测试先行的风格在系统设计上留下的痕迹。

<!-- There is also a benefit to system design. It is often very difficult to unit test some software systems. These systems are typically built code first and testing second, often by a different team entirely. By creating tests first your design will be influenced by a desire to test everything of value to your customer. Your design will reflect this by being easier to test.	 -->
 
这种先写测试的软件开发方式有其节奏感。你会先编写一个测试，描述手上要解决的一个小问题，然后编写[最简单的代码](simple-design.md)使测试通过；接着，再编写第二个测试，然后在刚刚的实现代码上再次编码，使新测试通过。但是注意不要过度实现！请通过新的测试来驱动实现。你应该重复这个过程，一直到所有需求全部变成测试用例、全部测试用例都通过为止。

<!-- There is a rhythm to developing software unit test first. You create one test to define some small aspect of the problem at hand. Then you create the simplest code that will make that test pass. Then you create a second test. Now you add to the code you just created to make this new test pass, but no more! Not until you have yet a third test. You continue until there is nothing left to test. The coffee maker problem shows an example written in Java. -->

测试驱动出来的代码往往十分简洁，仅仅实现你需要的功能。其他的开发者也可以通过浏览测试来了解代码的用法，在测试集中出现没有实际业务价值之测试的概率也会大大降低。

<!-- The code you will create is simple and concise, implementing only the features you wanted. Other developers can see how to use this new code by browsing the tests. Input whose results are undefined will be conspicuously absent from the test suite.  -->
