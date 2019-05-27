# DEAP 学习笔记

### Evolutionary Tools 进化工具

The tools module contains the operators for evolutionary algorithms. They are used to modify, select and move the individuals in their environment. The set of operators it contains are readily usable in the Toolbox. In addition to the basic operators this module also contains utility tools to enhance the basic algorithms with Statistics, HallOfFame, Checkpoint, and History.

工具模块包含进化算法的运算符。它们用于修改，选择和移动其环境中的个人。它包含的运算符集可以在工具箱中使用。除了基本操作符之外，该模块还包含实用工具，用于使用Statistics，HallOfFame，Checkpoint和History来增强基本算法。

#### Operators
The operator set does the minimum job for transforming or selecting individuals. This means, for example, that providing two individuals to the crossover will transform those individuals in-place. The responsibility of making offspring(s) independent of their parent(s) and invalidating the fitness is left to the user and is generally fulfilled in the algorithms by calling toolbox.clone() on an individual to duplicate it and del on the values attribute of the individual’s fitness to invalidate it.

操作员集完成转换或选择个人的最小工作。这意味着，例如，为交叉提供两个人将在适当的位置转换这些个体。让后代独立于其父母并使其适应性失效的责任留给用户，并且通常通过在个体上调用toolbox.clone（）来复制它并且在值属性上del来实现算法。个人的适合性使其失效。

Here is a list of the implemented operators in DEAP,

![image](http://blinkz.asuscomm.com:5000/d/f/489842199459012615)