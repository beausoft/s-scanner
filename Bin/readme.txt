s扫描器逆向修改加强版+源码 By http://www.dbgger.com/
版权归原作者WinEggDrop所有


TCP Port Scanner V1.2 By WinEggDrop

Usage:   s TCP/SYN StartIP [EndIP] Ports [Threads] [/T(N)] [/(H)Banner] [/Save]
Example: s TCP 12.12.12.12 12.12.12.254 80 512
Example: s TCP 12.12.12.12/24 80 512
Example: s TCP 12.12.12.12/24 80 512 /T8 /Save
Example: s TCP 12.12.12.12 12.12.12.254 80 512 /HBanner
Example: s TCP 12.12.12.12 12.12.12.254 21 512 /Banner
Example: s TCP 12.12.12.12 1-65535 512
Example: s TCP 12.12.12.12 12.12.12.254 21,3389,5631 512
Example: s TCP 12.12.12.12 21,3389,5631 512
Example: s SYN 12.12.12.12 12.12.12.254 80
Example: s SYN 12.12.12.12 1-65535
Example: s SYN 12.12.12.12 12.12.12.254 21,80,3389
Example: s SYN 12.12.12.12 21,80,3389

加入功能:

1: 支持http banner扫描 参数写为/HBanner即可
2: 支持TCP连接超时 加入/T(超时秒数即可) 如/T5指连接超时为5秒,如果不加，默认为原来的3秒
3: 加入域名解析功能，可直接指定域名
4: 加入网段指定功能，这个需要了解子网掩码的知识如 1.1.1.1/24指扫描1.1.1.1到1.1.1.254
   也可以直接用域名，如 s TCP www.163.com/24 80 512 /HBanner

优化了几处代码，压缩后仅7K大小

(保留原作者版权)
