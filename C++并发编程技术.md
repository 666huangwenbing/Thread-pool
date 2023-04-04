## C++并发编程技术

#### 并发与并行

Concurrent——并发：如果多个队列可以交替使用某台咖啡机，则这一行为就是并发的

Parallel——并行：如果存在多台咖啡机可以被多个队列交替使用，则就是并行



严格来说：如果一个系统支持多个动作同时存在，那么这个系统就是一个并发系统。如果这个系统还支持多个动作（物理时间上）同时执行，那么这个系统就是一个并行系统



#### 进程与线程

Process——进程：是指计算机中已运行的程序。进程为曾经是分时系统的基本运作单位。在面向进程设计的系统（如早期的UNIX，Linux 2.4及更早的版本）中，进程是程序的基本执行实体

Thread——线程：是操作系统能够进行运算调度的最小单位。它被包含在进程之中，是进程中的实际运作单位



![image-20230404092458144](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404092458144.png)



*Callable 类型是可以被执行调用操作的类型*：1.自定义函数 2.实例方法 3.迭代方法 4.异步方法 5.异步迭代方法  6.内置函数  7.内置方法  8.类  9.实例

![image-20230404092612968](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404092612968.png)



![image-20230404092929758](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404092929758.png)



**lambda表达式：**

![image-20230404093136181](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404093136181.png)

![image-20230404093406741](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404093406741.png)

![image-20230404093714098](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404093714098.png)

**注：lambda表达式底层是一个仿函数**



#### join与death

![image-20230404094205248](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404094205248.png)

![image-20230404094305175](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404094305175.png)



#### 管理当前进程

![image-20230404094425243](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404094425243.png)



#### 一次调用

![image-20230404094802626](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404094802626.png)

#### 竞争条件与临界区

![image-20230404095805759](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404095805759.png)

#### 互斥体与锁

![image-20230404095923354](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404095923354.png)

![image-20230404100114537](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404100114537.png)

![image-20230404100128015](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404100128015.png)

#### 通用的锁定算法

![image-20230404101142630](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404101142630.png)

#### 通用互斥管理

![image-20230404101329946](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404101329946.png)

**RALL**

![image-20230404101631885](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404101631885.png)



**条件变量**

![image-20230404101829902](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404101829902.png)

![image-20230404101854550](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404101854550.png)



**future**

![image-20230404102403143](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404102403143.png)

![image-20230404102507034](C:\Users\Admin\AppData\Roaming\Typora\typora-user-images\image-20230404102507034.png)



**借鉴连接**：https://paul.pub/cpp-concurrency/#id-ubuntu