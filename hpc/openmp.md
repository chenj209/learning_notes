## Openmp 性能优化

#### Cache contention

  * True sharing v.s. False sharing
    * True sharing: access to same variable
      Use private variable to make local copy
    * False sharing: access to same cacheline but different variable
      Data layout optimization to reduce false sharing
      共享cache不存在false sharing问题？
      Pay attention to page 56 of slides

#### NUMA aware programming
  * 线程绑定，处理相同数据应该使用同一个NUMA node下的线程

#### Synchronization
  * 消除不必要的隐式同步(nowait), check implicit barriers
