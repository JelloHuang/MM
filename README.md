* an asterisk starts an unordered list
* and this is another item in the list
+ or you can also use the + character
- or the - character

* Markdown

[Markdown Syntax Guide] http://sourceforge.net/p/kfn/wiki/markdown_syntax/#md_ex_bq
[GFM] http://github.github.com/github-flavored-markdown/

* what is per-cpu
Per-cpu data structure 在多核，多CPU或者多线程编程里面一个通用的技巧。
使用Per-cpu data  structure的目的是避免共享变量的锁，使得每个CPU可以独立访问数据而与其他CPU无关。
坏处是会  消耗大量的内存，而且并不是所有的变量都可以per-cpu化。并行是多核编程追求的目标，
而串行化  是多核编程里面最大的伤害。有关并行和串行的话题，在系统层次优化里面还会提到。
局部变量肯定是thread local的，所以在多核编程里面，局部变量反而更有好处。
per-cpu主要是为了解决SMP中锁占用的大量时间，而启用的一种机制。

kernel中的per_cpu变量 https://www.google.com.hk/search?q=kernel%E4%B8%AD%E7%9A%84per_cpu%E5%8F%98%E9%87%8F&sugexp=chrome,mod=12&sourceid=chrome&ie=UTF-8
