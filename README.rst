1.主要参考simple_cpu下的实现

2.参考 http://read.pudn.com/downloads102/ebook/417458/%E5%88%9D%E5%AD%A6cpu%E8%AE%BE%E8%AE%A1%EF%BC%88%E5%AE%8C%E5%85%A8%E6%95%99%E7%A8%8B%EF%BC%89/complexcpu_design.doc




=========================
ps.py:pipeline simulation
=========================

The node is a execution component that is defined with queue size and latency
(using step as unit).  the chain chains node as a line. The simulator is driven
by "step". We try to see how the executor stall and the change of the queue
unitilization.


spinlock.py: spin lock simulation
=================================

We assume there are n threads which share the same spinlock, we try to figure
out the behavior of the waiting queue

simple cpu
==========
this is a simple cpu simulator to show how cpu is work. see README.rst in the
directory for detail
