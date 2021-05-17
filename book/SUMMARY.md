# Summary

[引言](zh-cn/preface.md)

# [第一部分 基础篇](zh-cn/part1basic/readme.md)

- [第 1 章 Go 语言的前世今生](zh-cn/part1basic/ch01basic/readme.md)

  - [编程语言的发展](zh-cn/part1basic/ch01basic/history.md)
  - [Go 语言综述](zh-cn/part1basic/ch01basic/go.md)
  - [顺序过程通讯](zh-cn/part1basic/ch01basic/csp.md)
  - [Plan 9 汇编语言](zh-cn/part1basic/ch01basic/asm.md)

- [第 2 章 程序生命周期](zh-cn/part1basic/ch02life/readme.md)

  - [从 go 命令谈起](zh-cn/part1basic/ch02life/cmd.md)
  - [编译流程](zh-cn/part1basic/ch02life/compile.md)
  - [启动引导](zh-cn/part1basic/ch02life/boot.md)

- [第 3 章 语言核心](zh-cn/part1basic/ch03lang/readme.md)

  - [数组, 切片与字符串](zh-cn/part1basic/ch03lang/slice.md)
  - [散列表](zh-cn/part1basic/ch03lang/map.md)
  - [函数调用](zh-cn/part1basic/ch03lang/func.md)
  - [defer](zh-cn/part1basic/ch03lang/defer.md)
  - [panic/recover](zh-cn/part1basic/ch03lang/panic.md)
  - [通信原语](zh-cn/part1basic/ch03lang/chan.md)
  - [接口](zh-cn/part1basic/ch03lang/interface.md)
  - [运行时类型系统](zh-cn/part1basic/ch03lang/type.md)
  - [类型别名](zh-cn/part1basic/ch03lang/alias.md)
  - [进一步阅读的参考文献](zh-cn/part1basic/ch03lang/ref.md)

- [第 4 章 错误](zh-cn/part1basic/ch04errors/readme.md)

  - [问题的演化](zh-cn/part1basic/ch04errors/value.md)
  - [错误值检查](zh-cn/part1basic/ch04errors/inspect.md)
  - [错误格式与上下文](zh-cn/part1basic/ch04errors/context.md)
  - [错误语义](zh-cn/part1basic/ch04errors/semantics.md)
  - [错误处理的未来](zh-cn/part1basic/ch04errors/future.md)
  - [进一步阅读的参考文献](zh-cn/part1basic/ch04errors/ref.md)

- [第 5 章 同步](zh-cn/part1basic/ch05sync/readme.md)

  - [共享内存式同步模式](zh-cn/part1basic/ch05sync/basic.md)
  - [互斥](zh-cn/part1basic/ch05sync/mutex.md)
  - [原子操作](zh-cn/part1basic/ch05sync/atomic.md)
  - [条件变量](zh-cn/part1basic/ch05sync/cond.md)
  - [同步组](zh-cn/part1basic/ch05sync/waitgroup.md)
  - [缓存池](zh-cn/part1basic/ch05sync/pool.md)
  - [并发安全散列表](zh-cn/part1basic/ch05sync/map.md)
  - [上下文](zh-cn/part1basic/ch05sync/context.md)
  - [内存一致模型](zh-cn/part1basic/ch05sync/mem.md)
  - [进一步阅读的参考文献](zh-cn/part1basic/ch05sync/ref.md)

# [第二部分 运行时](zh-cn/part2runtime/readme.md)

- [第 6 章 调度器](zh-cn/part2runtime/ch06sched/readme.md)

  - [随机调度的基本概念](zh-cn/part2runtime/ch06sched/model.md)
  - [工作窃取式调度](zh-cn/part2runtime/ch06sched/steal.md)
  - [MPG 模型与并发调度单元](zh-cn/part2runtime/ch06sched/mpg.md)
  - [调度循环](zh-cn/part2runtime/ch06sched/schedule.md)
  - [线程管理](zh-cn/part2runtime/ch06sched/thread.md)
  - [信号处理机制](zh-cn/part2runtime/ch06sched/signal.md)
  - [执行栈管理](zh-cn/part2runtime/ch06sched/stack.md)
  - [协作与抢占](zh-cn/part2runtime/ch06sched/preemption.md)
  - [系统监控](zh-cn/part2runtime/ch06sched/sysmon.md)
  - [网络轮询器](zh-cn/part2runtime/ch06sched/poller.md)
  - [计时器](zh-cn/part2runtime/ch06sched/timer.md)
  - [非均匀访存下的调度模型](zh-cn/part2runtime/ch06sched/numa.md)
  - [进一步阅读的参考文献](zh-cn/part2runtime/ch06sched/ref.md)

- [第 7 章 内存分配](zh-cn/part2runtime/ch07alloc/readme.md)

  - [设计原则](zh-cn/part2runtime/ch07alloc/basic.md)
  - [组件](zh-cn/part2runtime/ch07alloc/component.md)
  - [初始化](zh-cn/part2runtime/ch07alloc/init.md)
  - [大对象分配](zh-cn/part2runtime/ch07alloc/largealloc.md)
  - [小对象分配](zh-cn/part2runtime/ch07alloc/smallalloc.md)
  - [微对象分配](zh-cn/part2runtime/ch07alloc/tinyalloc.md)
  - [页分配器](zh-cn/part2runtime/ch07alloc/pagealloc.md)
  - [过去、现在与未来](zh-cn/part2runtime/ch07alloc/history.md)

- [第 8 章 GC](zh-cn/part2runtime/ch08GC/readme.md)

  - [垃圾回收的基本想法](zh-cn/part2runtime/ch08GC/basic.md)
  - [写屏障技术](zh-cn/part2runtime/ch08GC/barrier.md)
  - [调步模型与强弱触发边界](zh-cn/part2runtime/ch08GC/pacing.md)
  - [扫描标记与标记辅助](zh-cn/part2runtime/ch08GC/mark.md)
  - [免清扫式位图技术](zh-cn/part2runtime/ch08GC/sweep.md)
  - [前进保障与终止检测](zh-cn/part2runtime/ch08GC/termination.md)
  - [安全点分析](zh-cn/part2runtime/ch08GC/safe.md)
  - [分代假设与代际回收](zh-cn/part2runtime/ch08GC/generational.md)
  - [请求假设与事务制导回收](zh-cn/part2runtime/ch08GC/roc.md)
  - [终结器](zh-cn/part2runtime/ch08GC/finalizer.md)
  - [过去、现在与未来](zh-cn/part2runtime/ch08GC/history.md)
  - [垃圾回收统一理论](zh-cn/part2runtime/ch08GC/unifiedgc.md)
  - [进一步阅读的参考文献](zh-cn/part2runtime/ch08GC/ref.md)

# [第三部分 工具](zh-cn/part3tools/readme.md)

- [第 9 章 分析](zh-cn/part3tools/ch09analysis/readme.md)

  - [死锁检测](zh-cn/part3tools/ch09analysis/deadlock.md)
  - [竞争检测](zh-cn/part3tools/ch09analysis/race.md)
  - [性能追踪](zh-cn/part3tools/ch09analysis/trace.md)
  - [代码测试](zh-cn/part3tools/ch09analysis/testing.md)
  - [基准测试](zh-cn/part3tools/ch09analysis/perf.md)
  - [运行时统计量](zh-cn/part3tools/ch09analysis/metric.md)
  - [语言服务协议](zh-cn/part3tools/ch09analysis/gopls.md)

- [第 10 章 依赖](zh-cn/part3tools/ch10deps/readme.md)

  - [依赖管理的难点](zh-cn/part3tools/ch10deps/challenges.md)
  - [语义化版本管理](zh-cn/part3tools/ch10deps/semantics.md)
  - [最小版本选择算法](zh-cn/part3tools/ch10deps/minimum.md)
  - [vgo 与 dep 之争](zh-cn/part3tools/ch10deps/fight.md)

- [第 11 章 编译](zh-cn/part3tools/ch11compile/readme.md)

  - [词法与文法](zh-cn/part3tools/ch11compile/parse.md)
  - [中间表示](zh-cn/part3tools/ch11compile/ssa.md)
  - [优化器](zh-cn/part3tools/ch11compile/optimize.md)
  - [指针检查器](zh-cn/part3tools/ch11compile/unsafe.md)
  - [逃逸分析](zh-cn/part3tools/ch11compile/escape.md)
  - [自举](zh-cn/part3tools/ch11compile/bootstrap.md)
  - [链接器](zh-cn/part3tools/ch11compile/link.md)
  - [汇编器](zh-cn/part3tools/ch11compile/asm.md)
  - [调用规约](zh-cn/part3tools/ch11compile/callconv.md)
  - [cgo 与系统调用](zh-cn/part3tools/ch11compile/cgo.md)

- [第 12 章 泛型](zh-cn/part3tools/ch12generics/readme.md)
  - [泛型设计的演进](zh-cn/part3tools/ch12generics/history.md)
  - [基于合约的泛型](zh-cn/part3tools/ch12generics/contracts.md)
  - [类型检查技术](zh-cn/part3tools/ch12generics/checker.md)
  - [泛型的未来](zh-cn/part3tools/ch12generics/future.md)
  - [进一步阅读的参考文献](zh-cn/part3tools/ch12generics/ref.md)

[结束语: Go 去向何处](zh-cn/finalwords.md)
[附录 A: 术语表](zh-cn/glossary.md)
