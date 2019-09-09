# 简单设计

相比于复杂的设计，简单的设计总是能花更短的时间实现。因此，在可工作的前提下，应该总是采用最简单的设计。如果你发现一些东西很复杂，那就使用更简单的方案替代它。对于复杂的代码，当下撤换它的成本总是最低的，通常也最快，否则将来它会浪费你更多的时间。

<!-- A simple design always takes less time to finish than a complex one. So always do the simplest thing that could possibly work next. If you find something that is complex replace it with something simple. It's always faster and cheaper to replace complex code now, before you waste a lot more time on it. -->

许多人热衷于对这种“简单性”进行度量。然而，“简单”与度量天生矛盾，因为简单是一种非常主观的品质。一个人眼中的简单，可能在第二个人眼中就显得复杂；引入一项高级的技术，可能简化一些应用的设计，却可能为其他的应用带来混乱。

<!-- Many people try to measure simplicity. Simple defies measurement because it is a very subjective quality. One person's simple is another person's complex. Adding an advanced technology can simplify one application and make a complete mess of another. -->

在项目中，“简单”的标准应该由团队自行确定，因为作为一个团队，你们需要一同对代码做出一致的评判。这里我向你推荐“简单”的四个主观特质以供参考：可测试（Testable）、可理解（Understandable）、可浏览（Browsable）、可解释（Explainable）（简称“[TUBE](http://www.zacharyspencer.com/2010/03/judging-code-simplicity-fit-it-through-the-tube/)”）。

<!-- Within your project the team decides what is simple. Together you judge your code subjectively. I recommend four subjective qualities; Testable, Understandable, Browsable, and Explainable (TUBE). -->

* **可测试**，意味着能够为代码编写自动化的单元测试及验收测试。这条原则会影响整体的设计，确保应用中的对象能互相解耦。你应该将系统分解成更小的可测试单元。

<!-- > Testable means you can write unit tests and acceptance tests to automatically check for problems. This impacts the overall design and coupling of objects in your application. Break your system into small testable units. -->

* **可浏览**，是指需要找寻某些东西时，能够顺利找到它。好的名字对搜索至关重要。同样，正确地使用多态、委托、继承，也能帮助你在需要寻找时有迹可循。

<!-- > Browsable is the quality of being able to find what you want when you want it. Good names helps you find things. Using polymorphism, delegation, and inheritance correctly helps you find things when you need to. -->

* **可理解**，意思很直白了。但“可理解”本身也带有很强的主观性。如果一个团队长时间工作在一个系统上，他们应该能很容易理解该系统；但新加入的成员则可能一头雾水。因此，我同时也推荐将“**可解读**”作为一项品质：你应当能轻松地向新人介绍系统运作的原理。

<!-- > Understandable is obvious, but highly subjective. A team that has been working with a system a long time will understand it even though someone new is completely baffled. So I also recommend explainable as a quality that means it's easy to show new people how everything works. -->

有很多人喜欢用这个方法衡量系统是否简单：“一次，并且至多一次”。这句话其实有两个部分，似乎大家都能理解“至多一次”的部分，但对前半句“一次”则缺乏关注。实际上，前半句的意思是：应该完整地表达代码的所有意图，哪怕完整表达可能带来代码的重复。

<!-- > Many people recommend a measure of simplicity as: Once and only once. It is important to remember this has two parts. Everyone seems	to understand the "only once" part but not the "once and" part. The first part means express all the intention of your code even if it means duplication. -->

试看一个简单的例子：将一个分数转换成百分比时，你需要将该数乘以100；将一个单位为“米”的数字转换成“厘米”时，你同样需要将该数乘以100。那么，你是否应该将这段“乘以100”的逻辑提炼成为一个单独的函数`convertToPercentOrMeters(x)`呢？显然不应该！即便因此消除了一些重复，也不应该这样做。你需要的是两个方法：`convertToPercent(aFraction)`以及`convertMetersToCentimeters(aLength)`，因为它们表达的是不同的意图。尽管存在“乘以100”的表面重复，但它们乘100背后的动机是不同的，各自所需的数字类型也是不同的。

<!-- > Consider a simple example; you multiply by 100 to turn a fraction into percentage and you also multiply by 100 to turn meters into centimeters. Should you have a single function that multiplies by 100 called convertToPercentOrMeters(x)? NO! Not even if it would remove some duplication. You want two methods; converToPercent(aFraction), and convertMetersToCentimeters(aLength). You want two because they tell you different things. Not just that you will multiply by 100 but also why you will multiply by 100 and what kinds of numbers are valid inputs. -->

此外，进行简单的设计需要知识的支撑。知识不同于信息：你可能了解许多信息，却没有太多有益的知识。知识，是指对你日常处理的问题域，经过时间沉淀而形成的深入洞察。

<!-- > One thing about simple designs is that they require knowledge to recognize. Knowledge is different from information, you can have plenty of information and no knowledge. Knowledge is insight into your problem domain that develops over time. -->

简单的设计往往在项目开展一段时间后才会涌现。促成简单设计的最佳做法是：一面仅为必须实现的功能编写代码，一面积极为简单的设计寻求必要的知识。一旦对设计有了新的理解，就可以渐进地往那个方向进行重构。

<!-- > Simple designs often come after the project has been running for a while. The best approach is to create code only for the features you are implementing while you search for enough knowledge to reveal the simplest design. Then refactor incrementally to implement your new understanding and design. -->

绝不在真正需要某项功能之前实现它，如此方能维护设计的长期简洁。即便如此也仍然要明白：保持简单的设计需下苦功，不可能一蹴而就。

<!-- > Keep things as simple as possible as long as possible by never adding functionality before it is scheduled. Beware though, keeping a design simple is hard work. -->
