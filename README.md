硬盘上的第一个512个字节
    

这个512字节就是硬盘的主引导扇区，它包括，一个简短的引导程序，一个分区表。在硬盘引导的情况下，BIOS自检完成后，就把这512个字节调入内存，并把CPU的控制权交给它。该引导程序读取分区表，确定一个可引导分区，并把分区的第一个扇区(512字节)读入内存，然后把CPU的控制权交给它，继续完成最终的系统引导。

硬盘的这种设计，是为了使一个硬盘可以同时安装多个操作系统。

程序大概写于97年，那是一个还使用软驱的时代，XP还要很久才诞生。99年整理发布到了网上，如今在一些代码网站仍能搜索到。也许还有点用，现在重新收集，并制作了一个DOS系统的VirtualBox虚拟盘，放到github上方便各位玩耍。

更多详情，请查阅原[readme.txt](https://raw.githubusercontent.com/optman/bootmaster/master/readme.txt)文档。

![alt tag](https://raw.githubusercontent.com/optman/bootmaster/master/bootmenu.png)



2014/4/23

     