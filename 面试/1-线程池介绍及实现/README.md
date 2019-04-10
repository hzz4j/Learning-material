
[线程池的介绍及简单实现](https://www.ibm.com/developerworks/cn/java/l-threadPool/index.html#icomments)

WorkThread线程在taskVector没有任务时，就处于wait状态，
当taskVector有任务要处理时，线程就会去执行他，
其实CalculationTaskTest实现Task并不一定要实现runnable
Task接口的好处是，解耦合，能够使得WorkThread直接操作Task接口


