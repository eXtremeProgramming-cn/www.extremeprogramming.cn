<!-- When a bug is found tests are created to guard against it coming back. A bug in production requires an acceptance test be written to guard against it. Creating an acceptance test first before debugging helps customers concisely define the problem and communicate that problem to the programmers. Programmers have a failed test to focus their efforts and know when the problem is fixed.

Given a failed acceptance test, developers then create unit tests to show the defect from a more source code specific point of view. Failing unit tests give immediate feedback to the development effort when the bug has been repaired. When the unit tests run at 100% then the failing acceptance test can be run again to validate the bug is fixed.  -->

# 缺陷管理

每次发现Bug，需要建立相应的测试以防止Bug再现。产品中的Bug，需要写一个验收测试来防止再次出现。发现Bug后，不要急于着手调试，首先为其创建一个验收测试，这样可以帮助客户简洁地定义问题、并将问题传达给程序员。有一个失败的测试在手，程序员就可以专注于修复这个测试，并且清晰知道问题是否得到了修复。

有了一个失败的验收测试之后，开发人员可以创建单元测试，从深入源代码的角度展示缺陷的存在。失败的单元测试可以给开发人员更加迅速的反馈，以便知道Bug是否被修复了。当单元测试100%通过后，我们就可以再次运行验收测试，确认Bug是否得到修复。
