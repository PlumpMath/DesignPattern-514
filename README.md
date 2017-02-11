# DesignPattern
设计模式总结-java版

﻿> 参考： 
	《head first设计模式》的官方代码
	http://download.csdn.net/detail/undergrowth/8306683
	


## OO设计原则：
	- 封装变化
	- 多用组合，少用继承
	- 针对接口编程，不针对实现编程
	- 对交互对象之间的松耦合设计而努力
	- 对扩展开方，对修改关闭(例如: 装饰者模式)
	- 依赖抽象，不要依赖具体类(例如：工厂模式)
	- 最少知识原则：只和你的密友交谈

## OO设计模式：

### 策略者设计模式：
	  将算法簇封装起来，使使用算法的客体和算法之间相互独立
### 观察者设计模式：

### 装饰者设计模式：
	  不改变接口，但动态的加入责任。装饰者提供有别于继承的另一种选择，比继承更具有扩展性。(例如：java.IO包)

### 适配器模式
      将一个或多个接口改变为用户所期望的另一个接口。

### 外观模式
      提供了系统的一个简化的高层接口，用来简化访问系统的一群接口

### 工厂设计模式：

#### 	简单工厂模式：
		  在一个类中处理创建对象的细节。
####    工厂方法模式：
		  定义了一个创建**对象**的接口，但由子类决定要实例化的类是哪一个。工厂方法让类把实例化推迟到子类。
####    抽象工厂模式：
		  提供一个接口，用于创建相关或依赖对象的**家族**，而不需要明确指定具体类。

### 单例模式
      确保类只有一个实例，并提供一个全局的访问点

### 命令模式
      将请求封装成对象，使不同的请求、日志、队列来参数化其他对象。

### 模板方法模式
	   定义了一个算法的框架，允许继承的子类为其提供一个或多个步骤的实现方法或可选的实现方法(hook)

	   - 模板方法和策略方法都封装算法，模板使用继承，策略使用组合

### 迭代器模式
	   提供一种顺序访问聚合对象元素的方法，而又不暴露其内部元素, 迭代器将遍历聚合对象的任务封装到一个对象(可以是聚合对象中也可以是自定义的迭代器对象)中。

### 组合模式
	   允许你将对象组成树形结构来表现“整体/部分”的层次结构。组合能让客户以一致的方式处理个别对象和对象组合。

### 状态模式：
       允许对象在内部状态改变时改变他的行为，对象看起来好像修改了他的类

### 代理模式：
	   给真实对象提供一个替身，以控制对这个对象的访问  

	- 装饰者为对象增加额外的行为，而代理是控制对象的访问。
	- 适配器和代理都是挡在其他对象的前面，并负责将请求转发给他们。适配器会提供不同的接口用于适配，而代理则实现相同的接口。
	- 外观模式是包装许多对象以简化他们的接口
