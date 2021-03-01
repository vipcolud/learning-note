# 规则引擎
## 使用场景

对于多分支的if else，可以使用策略模式进行优化。但是对于过多分支的情况，会使得策略过多，难以维护。

在该种情况下，需求点为以下四点：
- 第一，我们要简化if else结构,让业务逻辑和数据分离！
- 第二，分离出的业务逻辑必须要易于编写，至少单独编写这些业务逻辑，要比写代码快！
- 第三，分离出的业务逻辑必须要比原来的代码更容易读懂！
- 第四，分离出的业务逻辑必须比原来的易于维护，至少改动这些逻辑，应用程序不用重启！

规则引擎满足以上的需求点，具体体现在如下：
![image](https://github.com/rbmonster/learning-note/blob/master/src/main/java/com/learning/other/picture/ruleEnginExample.jpg)

参考资料：[规则引擎的使用场景](https://www.cnblogs.com/rjzheng/p/10996186.html)


使用规则引擎可以给系统带来如下优势：
- 高灵活性：在规则保存在知识库中，可以在规则变动轻易做出修改。
- 容易掌控：规则比过程代码更易于理解，因此可以有效地来弥补业务分析师和开发人员之间的沟通问题。
- 降低复杂度：在程序中编写大量的判断条件，很可能是会造成一场噩梦。使用规则引擎却能够通过一致的表示形式，更好的处理日益复杂的业务逻辑。
- 可重用性：规则集中管理，可提高业务的规则的可重用性。而且，传统的代码程序通常会添加不必要的变数，很然进行重复利用。
> 需要留意的是，在业务规则没有太多变动，业务规则比较简单的情况下，是没有必要使用规则引擎的。