# Fragment生命周期

## androidx
MainActivity + Fragment1 演示了androidx下的fragment生命周期，见log日志打印
- 这种方式的fragment构造函数可以传入布局ID，无需在fragment中再写了。

## sdk原生
MainActivity2 + Fragment2 演示了原生sdk下的fragment生命周期，见log日志打印
- 这种方式的fragment构造函数不能传入布局ID，只能无参，在fragment中自己写inflate语句。

## 共同点
如果不声明fragment布局，那么onViewCreated函数就不会执行。
如果声明了布局，则onViewCreated函数会执行，返回的view和onCreateView中的是同一个对象。
