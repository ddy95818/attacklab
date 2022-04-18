*************************
做题之前先阅读attacklab.pdf
*************************

This file contains materials for one instance of the attacklab.

Files:

    ctarget --- 代码注入的攻击目标文件

Linux binary with code-injection vulnerability.  To be used for phases 1-3 of the assignment.

    rtarget --- ROP攻击目标的文件
                return-oriented programming 面向返回的编程：
                                            攻击者扫描已有的动态库链接和可执行文件，提取出可以利用的指令片段
                                            这些指令片段均已ret指令结尾
                                            即用ret指令实现指令片段执行流的衔接

Linux binary with return-oriented programming vulnerability.  To be used for phases 4-5 of the assignment.

     cookie.txt --- 一个4字节的十六进制数，作为攻击的特殊标志符

Text file containing 4-byte signature required for this lab instance.

     farm.c

Source code for gadget farm present in this instance of rtarget.  You can compile (use flag -Og) and disassemble it to look for gadgets.

     hex2raw --- 将十六进制转换为攻击字符
     ./hex2raw <level1.txt> level1

Utility program to generate byte sequences.  See documentation in lab handout.
