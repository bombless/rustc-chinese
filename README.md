# Rust 编程语言

这里是一个使用中文输出错误的 Rust 编译器，
包括标准库，工具，还有文档。
Rust 是一个高效、内存安全、并行的系统编程语言，
同时不使用一个垃圾收集器或其他强加的大的运行时负担。

## 从源码编译

1. 确保你已经安装了以下依赖：

   * `g++` 4.7 或 `clang++` 3.x
   * `python` 2.6 或更新 （但不能是 3.x）
   * GNU `make` 3.81 或更新
   * `curl`
   * `git`

2. 用 `git` 克隆 [源码]：

   ```sh
   $ git clone https://github.com/bombless/rustc-chinese.git
   $ cd rust
   ```

[源码]: https://github.com/bombless/rustc-chinese

3. 构建并安装：

    ```sh
    $ ./configure
    $ make && make install
    ```

### 在 Windows 上构建

可以用 [MSYS2](http://msys2.github.io/) 来轻松构建本项目：

1. 拿到最新的 MSYS2 安装程序并安装。

2. 从 MSYS2 控制台安装 `mingw64` 工具链及其他需要的工具。

   ```sh
   # 工具平台选一个
   $ pacman -S mingw-w64-i686-toolchain
   $ pacman -S mingw-w64-x86_64-toolchain

   $ pacman -S base-devel
   ```

3. 根据你想要 32 位或 64 位 Rust 从 MSYS2 安装目录运行 `mingw32_shell.bat` 或
`mingw64_shell.bat`。

4. 转到源码路径，配置并构建

   ```sh
   $ ./configure
   $ make && make install
   ```

## 获得帮助

Rust 中文社区的人们在几个地方聚集：

* [rust.cc] - Rust 中文社区讨论论坛
* [v2ex] - V2EX Rust 节点
* [知乎] - 问答

[rust.cc]: http://rust.cc/
[v2ex]: http://v2ex.com/go/rustlang
[知乎]: http://www.zhihu.com/topic/19674381

## License

Rust is primarily distributed under the terms of both the MIT license
and the Apache License (Version 2.0), with portions covered by various
BSD-like licenses.

See [LICENSE-APACHE](LICENSE-APACHE), [LICENSE-MIT](LICENSE-MIT), and [COPYRIGHT](COPYRIGHT) for details.
