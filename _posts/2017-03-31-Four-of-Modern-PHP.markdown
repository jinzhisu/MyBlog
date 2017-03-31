---
layout: post
title:  "Four of Modern PHP"
date:   2017-03-31
categories: Tranlation

---

1. Today, the PHP language is quickly evolving and is supported by dozens of core team developers from around the world.

    今天，PHP 经由来自于全世界的数十名核心开发者的支持快速的发展着。

2. Development practices have changed, too.

    开发模式也已发生了改变。
    
3. In the past, it was common practice to write a PHP file, upload it to a production server with FTP, and hope it worked.

    在过去，通常的做法是编写PHP代码文件，然后通过FTP上传到生产服务器上，并且期望它能够工作。
    
4. This is a terrible development strategy, but it was necessary due to a lack of viable local development environments.

    这是一种开发的开发策略，但又别无他法，由于当时缺乏可行的本地开发环境。
    
5. Nowadays, we eschew FTP and use version control instead.

    现如今，我们避开FTP转而使用版本控制系统代替。
    
6. Version control software like Git helps maintain an auditable code history that can be branched, forked, and
merged.

    像Git一样的版本控制系统帮助记录审核代码历史，并且能够对其建立分支，拷贝以及合并。

7. Local development environments are identical to production servers thanks to virtualization tools like Vagrant and provisioning tools like Ansible, Chef, and
Puppet.

    本地的开发环境与生产环境保持一致，这得益于虚拟化工具例如Vagrant和配置工具例如 Ansibl ，Chef 以及 Puppe。

8. We leverage specialized PHP components with the Composer dependency manager.

    我们借助于 Composer 依赖管家使用特殊的PHP组件。
    
9. Our PHP code adheres to PSRs—community standards managed by the PHP Framework Interop Group.

    我们的PHP代码遵循 PSRs-由 PHP Framework Interop Group 制定的社区标准。
    
10. We thoroughly test our code with tools like
PHPUnit.

    我们使用像 PHPUnit 这样的工具深入测试我们的代码。
    
11. We deploy our applications with PHP’s FastCGI process manager behind a web server like nginx.

    我们使用 PHP 的 FastCGI 进程管家部署自己的应用程序在像 nginx 这样的 Web 服务器之后。
    
12. And we increase application performance with an opcode cache.

    并且我们使用 opcode 缓存提升应用程序的性能。
    
13. Modern PHP encompasses many new practices that may be unfamiliar to those of you new to PHP, or to those upgrading from older PHP versions.

    你或许从刚刚接触PHP，或许由旧的版本升级而来，现代PHP对你而言可能有一些陌生。
    
14. Don’t feel overwhelmed.

    不要感觉到不知所措。
    
15. I’ll walk through each concept later in this book.

    本书稍后将介绍每个概念。
    
16. I’m also excited that PHP now has an official draft specification—something it lacked until 2014.

    我为PHP能有一份官方的规范草案而感到高兴，在2014年以前是没有的。
