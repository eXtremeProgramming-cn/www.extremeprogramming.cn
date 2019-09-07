<!--
	When a bug is found tests are created to guard against it coming back. A bug in production requires an acceptance test be written to guard against it. Creating an acceptance test first before debugging helps customers concisely define the problem and communicate that problem to the programmers. Programmers have a failed test to focus their efforts and know when the problem is fixed.
 Given a failed acceptance test, developers then create unit tests to show the defect from a more source code specific point of view. Failing unit tests give immediate feedback to the development effort when the bug has been repaired. When the unit tests run at 100% then the failing acceptance test can be run again to validate the bug is fixed. 
--!>
# Bug
 当一个Bug被发现后，需要建立相应的测试以防止Bug再现。产品中的Bug，需要写一个验收测试用来防止。发现Bug后，在调试之前先创建一个验收测试可以帮助客户简洁地定义问题并将该问题传达给程序员。程序员就有了一个失败的测试，这样他们可以知道什么时候修复了它。

 有了一个失败的验收测试，开发人员就可以从源代码的角度创建单元测试用来展示缺陷。失败的单元测试，可以给开发人员更加迅速的反馈以便知道Bug是否被修复了。当单元测试100%通过后，我们就可以再次运行验收测试，确认Bug是否被修复。

 翻译：邓志国 bobdeng@163.com