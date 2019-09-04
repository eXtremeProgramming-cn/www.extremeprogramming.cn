# 简单设计

简单的设计总是比复杂的设计花更少时间实现。因此，在可工作的前提下，应该总是采用最简单的设计。如果你发现一些东西很复杂，那就使用更简单的方案取代它。对于复杂的代码，马上撤换它的成本总是最低的，也会更快，否则以后它会浪费你更多的时间。

> A simple design always takes less time to finish than a complex one. So always do the simplest thing that could possibly work next. If you find something that is complex replace it with something simple. It's always faster and cheaper to replace complex code now, before you waste a lot more time on it.

许多人热衷于定量地衡量“简单性”。然而，？，因为简单是种非常主观的品质。一个人眼中的简单，可能在另个眼中却显得复杂；引入一项高级的技术，可能简化一些应用的设计，却可能对其他的应用带来混乱。

> Many people try to measure simplicity. Simple defies measurement because it is a very subjective quality. One person's simple is another person's complex. Adding an advanced technology can simplify one application and make a complete mess of another.
 
在项目中，你的团队应该自行决定“何谓简单”，？。这里我向你推荐“简单”的四个特质，当然这是我的主观看法：可测试（Testable）、可理解（Understandable）、可预览（Browsable）、可解释（Explainable）（简称TUBE）。
 
> Within your project the team decides what is simple. Together you judge your code subjectively. I recommend four subjective qualities; Testable, Understandable, Browsable, and Explainable (TUBE).

可测试，意味着有可能为代码编写自动化的单元测试及验收测试。这条原则会影响整体的设计，确保应用中的对象能互相解耦。你的系统应该被分解成更小的可测试单元。

可预览，是指需要找寻某些东西时，有可能正常找到它。好的名字对搜索至关重要。同样，正确地使用多态、委托、继承，也能帮助你在需要时有迹可循。

可理解，顾名思义。但“可理解”本身也带有很强的主观性。如果一个团队长时间工作在一个系统上，他们应该能很容易理解该系统——但新加入的成员则可能一头雾水。因此，我同时也推荐将“可解释”作为一项品质：你应当能轻松地向新人介绍系统运作的原理。

有很多人喜欢用这个方法衡量系统是否“简单”：Once and only once. 这句话其实有两个部分，大家似乎只看到“only once”的后半句，但对前半句“once and”则缺乏理解。而实际上，前半句指出：完整地表达代码的所有意图，哪怕完整表达会带来代码重复。

> Many people recommend a measure of simplicity as: Once and only once. It is important to remember this has two parts. Everyone seems	to understand the "only once" part but not the "once and" part. The first part means express all the intention of your code even if it means duplication.

试看一个简单的例子：将一个分数转换成百分比时，你需要将该数乘以100；将一个单位为“米”的数字转换成“厘米”时，你同样需要将该数乘以100。那么，你是否应该将这段“乘以100”的逻辑提炼成为一个单独的函数`convertToPercentOrMeters(x)`呢？显然不应该！即便因此消除了一些重复，也不应该这样做。你需要的是两个方法：`convertToPercent(aFraction)`以及`convertMetersToCentimeters(aLength)`，因为它们表达的是不同的意图。尽管存在“乘以100”的表面重复，但它们乘100背后的动机是不同的，各自所需的数字类型也是不同的。

> One thing about simple designs is that they require knowledge to recognize. Knowledge is different from information, you can have plenty of information and no knowledge. Knowledge is insight into your problem domain that develops over time.
 
> Simple designs often come after the project has been running for a while. The best approach is to create code only for the features you are implementing while you search for enough knowledge to reveal the simplest design. Then refactor incrementally to implement your new understanding and design.
 
> Keep things as simple as possible as long as possible by never adding functionality before it is scheduled. Beware though, keeping a design simple is hard work.
 
