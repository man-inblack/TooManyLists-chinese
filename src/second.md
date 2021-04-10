# 一个还不错的单链栈

在前一章中我们写了一个轻量级可行的单链栈。然而其中的一些设计上的抉择使它成了一个比较糟糕的栈。这一章，让我们使它变得不那么糟糕些。为了达成目标，我们需要做的有：

* {重新造轮子}
* 使我们的列表可以处理任意的元素类型
* 支持Peek方法
* 使我们的列表可以迭代

在这一过程中我们将学到

* Option的进阶用法
* 泛型
* 生命周期
* 迭代器

我们来新建一个`second.rs`文件:

```rust ,ignore
// in lib.rs

pub mod first;
pub mod second;
```

然后将上一章的`first.rs`中的所有代码复制到新建的文件中。