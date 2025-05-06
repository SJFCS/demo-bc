复式簿记系统中，一般有五个大桶，每个桶里又可以放很多个小桶，这五个大桶分别是：

- 资产 Assets: 现金、银行存款、有价证券等；
- 负债 Liabilities: 信用卡、房贷、车贷等；
- 收入 Income: 工资、奖金等；
- 费用 Expenses: 外出就餐、购物、旅行等；
- 权益 Equity: 用于「存放」某个时间段开始前已有的豆子，下文详述。

与传统的复式簿记不同，Beancount 及其前辈们用的复式簿记方法使用了正负号而不是拗口的「借」（debit）和「贷」（credit）来表示五个桶之间的豆子变动，更加容易理解和思考，也不容易出错。本文所介绍的复式簿记采用 Beancount 的方案。

- [Beancount -- Language Syntax](https://docs.google.com/document/d/1wAMVrKIA2qtRGmoVDSUBJGmYZSygUaR0uOMW1GV3YE0/)
- [Beancount -- Getting Started](https://docs.google.com/document/d/1P5At-z1sP8rgwYLHso5sEy3u4rMnIUDDgob9Y_BYuWE/)
- [Beancount -- Syntax Cheat Sheet](https://docs.google.com/document/d/1M4GwF6BkcXyVVvj4yXBJMX7YFXpxlxo95W6CpU3uWVc/)

**每笔交易在不同账户的数字加起来和为 0 是复式簿记的重要特性和原则，也是用来检验账目正确性的重要依据。**

- 把收入（Income）想像成一个装着你一生（过去和未来）所有劳动成果的桶，每次你的收入都是从桶里取出东西（通常以货币的形式），一直取啊取啊，直到某一天......所以**收入桶的数字通常是负数**。
- 把费用（Expenses）想像成一个装着你一生（过去和未来）所有消费的桶，每次你的支出都是往桶里放东西（以货币的形式表现），和朋友出去唱歌转换成快乐存进去，看过的电子书转换成精神食粮存进去，吃过的饭转换成......所以**费用桶的数字通常是正数**。

(Income + Liabilities) + (Assets + Expenses) + Equity = 0
