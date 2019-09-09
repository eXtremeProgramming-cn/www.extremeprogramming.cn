# CRC卡

借助CRC（即：Class - 类名、Responsibilities - 类的职责、Collaboration - 类的协作关系）卡，团队可以共同设计系统。CRC卡最大的价值是让人们摆脱程序化的思维模式，更充分地利用对象技术。CRC卡允许整个项目团队成员参与设计。能够帮助设计系统的人越多，好点子的数量就越多。

每张CRC卡表示一个对象。可以把该对象所属的类写在卡片的顶部、类的职责列在左边、与其协作的类列在每个职责的右边。之所以说“可以”，是因为一旦CRC相关的讨论开启，参与者通常只需要一些带有类名的卡片，不需要完整地写出卡片。

围绕CRC卡，团队会讨论“哪些对象向其他对象发送消息”，这就是在模拟系统的行为。随着讨论逐步深化，很容易发现缺点和问题。通过模拟各种设计方案，可以快速探索各个方案的优劣。

如果你发现太多的人同时说话和移动卡片，那么可以限制站着移动卡片的人数，例如规定只有两个人能站起来移动卡片。只有当前一个人坐下时，另一个人才能站起来。这对于失控的会话有奇效。

对CRC卡最大的批评之一是缺乏书面设计。但通常你并不需要更详尽的书面设计文档，因为CRC卡使设计显而易见。如果需要更持久的记录，可以为每个类写一张完整的卡片，并作为文档保存。


<!-- # CRC Cards
Use Class, Responsibilities, and Collaboration (CRC) Cards to design the system as a team. The biggest value of CRC cards is to allow people to break away from the procedural mode of thought and more fully appreciate object technology. CRC Cards allow entire project teams to contribute to the design. The more people who can help design the system the greater the number of good ideas incorporated.

Individual CRC Cards are used to represent objects. The class of the object can be written at the top of the card, responsibilities listed down the left side, collaborating classes are listed to the right of each responsibility. We say "can be written" because once a CRC session is in full swing participants usually only need a few cards with the class name and virtually no cards written out in full. A short example is shown as part of the coffee maker problem.

A CRC session proceeds with someone simulating the system by talking about which objects send messages to other objects. By stepping through the process weaknesses and problems are easily uncovered. Design alternatives can be explored quickly by simulating the design being proposed.

If you find too many people speaking and moving cards at once then simply limit the number of people standing and moving cards to two. When one person sits down another may stand up. This works for sessions that get out of hand, which often happens as teams become rowdy when a tough problem is finally solved.

One of the biggest criticisms of CRC Cards is the lack of written design. This is usually not needed as CRC Cards make the design seem obvious. Should a more permanent record be required, one card for each class can be written out in full and retained as documentation. A design, once envisioned as if it were already built and running, stays with a person for some time.
-->