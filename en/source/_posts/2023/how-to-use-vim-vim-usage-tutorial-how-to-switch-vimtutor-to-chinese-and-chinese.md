---
title: vim怎么使用，vim使用教程，vimtutor怎么切换中文 汉化
subtitle: How to use vim, vim usage tutorial, how to switch vimtutor to Chinese and Chinese
date: 2023-08-02 19:26:52
toc: true
categories: 
    - 默认
---

# vim怎么使用，vim使用教程，vimtutor怎么切换中文 汉化

# vim 使用

> 在安装了 vim 的 unix 系统下可以使用 `vimtutor zh_cn` 开启下面的教程

## 序言

```zsh
===============================================================================
=      欢     迎     阅     读   《 V I M  教  程 》   ——      版本 1.7       =
===============================================================================

     Vim 是一个具有很多命令的功能非常强大的编辑器。限于篇幅，在本教程当中
     就不详细介绍了。本教程的设计目标是讲述一些必要的基本命令，而掌握好这
     些命令，您就能够很容易地将 Vim 当作一个通用编辑器来使用了。

     完成本教程的内容大约需要25-30分钟，取决于您训练的时间。

     注意：
     每一节的命令操作将会更改本文。推荐您复制本文的一个副本，然后在副本上
     进行训练(如果您是通过"vimtutor"来启动教程的，那么本文就已经是副本了)。

     切记一点：本教程的设计思路是在使用中进行学习的。也就是说，您需要通过
     执行命令来学习它们本身的正确用法。如果您只是阅读而不操作，那么您可能
     会很快遗忘这些命令的！

     好了，现在请确定您的Shift-Lock(大小写锁定键)还没有按下，然后按键盘上
     的字母键 j 足够多次来移动光标，直到第一节的内容能够完全充满屏幕。
```

## 第一讲第一节：移动光标

```zsh
             ** 要移动光标，请依照说明分别按下 h、j、k、l 键。 **

             ^
             k              提示： h 的键位于左边，每次按下就会向左移动。
       < h       l >               l 的键位于右边，每次按下就会向右移动。
             j                     j 键看起来很象一支尖端方向朝下的箭头。
             v

  1. 请随意在屏幕内移动光标，直至您觉得舒服为止。

  2. 按下下行键(j)，直到出现光标重复下行。

---> 现在您应该已经学会如何移动到下一讲吧。

  3. 现在请使用下行键，将光标移动到第一讲第二节。

提示：如果您不敢确定您所按下的字母，请按下<ESC>键回到正常(Normal)模式。
      然后再次从键盘输入您想要的命令。

提示：光标键应当也能正常工作的。但是使用hjkl键，在习惯之后您就能够更快
      地在屏幕内四处移动光标。真的是这样！
```

**注意**

`hjkl`并不是特定单词的缩写。这些字符`h`、`j`、`k`、`l`仅仅是为了方便在Vim编辑器中表示上下左右方向而选定的按键。它们没有特定的含义或单词背后的缩写。

## 第一讲第二节：VIM的进入和退出

```zsh
  !! 特别提示：敬请阅读本一节的完整内容，然后再执行以下所讲解的命令。

  1. 按<ESC>键(这是为了确保您处在正常模式)。

  2. 然后输入：                 :q! <回车>
     这种方式的退出编辑器会丢弃您进入编辑器以来所做的改动。

  3. 如果您看到了命令行提示符，请输入能够带您回到本教程的命令，那就是：
     vimtutor <回车>

  4. 如果您自信已经牢牢记住了这些步骤的话，请从步骤1执行到步骤3退出，然
     后再次进入编辑器。

提示： :q! <回车> 会丢弃您所做的任何改动。几讲之后您将学会如何保存改动到文件。

  5. 将光标下移到第一讲第三节。
```

**注意**

`q` 是 `quit`（退出）单词缩写

## 第一讲第三节：文本编辑之删除

```zsh
   ** 在正常(Normal)模式下，可以按下 x 键来删除光标所在位置的字符。**

  1. 请将光标移动到本节中下面标记有 ---> 的那一行。

  2. 为了修正输入错误，请将光标移至准备删除的字符的位置处。

  3. 然后按下 x 键将错误字符删除掉。

  4. 重复步骤2到步骤4，直到句子修正为止。

---> The ccow jumpedd ovverr thhe mooon.

  5. 好了，该行已经修正了，下面是第一讲第四节。

特别提示：在浏览本教程时，不要强行记忆。记住一点：在使用中学习。
```

## 第一讲第四节：文本编辑之插入

```zsh
         ** 在正常模式下，可以按下 i 键来插入文本。**

  1. 请将光标移动到本节中下面标记有 ---> 的第一行。

  2. 为了使得第一行内容雷同于第二行，请将光标移至文本第一个准备插入字符
     的位置。

  3. 然后按下 i 键，接着输入必要的文本字符。

  4. 每个错误修正完毕后，请按下 <ESC> 键返回正常模式。
     重复步骤2至步骤4以便修正句子。

---> There is text misng this .
---> There is some text missing from this line.

  5. 如果您对文本插入操作已经很满意，请接着阅读下面的第一讲第五节。
```

**注意**

`i` 是 `insert`（插入）单词的缩写

I键（小写）：在当前光标所在字符的前面进入插入模式。

按下I键后，光标会保持在当前字符的位置，然后你可以开始输入新的文本。这对于在行的任何位置开始添加内容很有用。

## 第一讲第五节：文本编辑之添加

```zsh
                        ** 按 A 键以添加文本。 **

  1. 移动光标到下面第一个标记有 ---> 的一行。
     光标放在那一行的哪个字符上并不重要。

  2. 按 A 键输入必要的添加内容。

  3. 文本添加完毕后，按 <ESC> 键回到正常模式。

  4. 移动光标到下面第二个标记有 ---> 的一行。重复步骤2和步骤3以改正这个句子。

---> There is some text missing from th
     There is some text missing from this line.
---> There is also some text miss
     There is also some text missing here.

  5. 当您对添加文本操作感到满意时，请继续学习第一讲第六节。
```

**注意**

`a` 是 `append`（添加）单词的缩写

A键（小写）：在当前光标所在字符的后面进入插入模式。

按下A键后，光标会移动到当前行的末尾，然后你可以开始输入新的文本。这对于在行的末尾添加内容很方便。

## 第一讲第六节：编辑文件

```zsh
                    ** 使用 :wq 以保存文件并退出。 **

  特别提示：在执行以下步骤之前，请先读完整个小节！

  1. 如您在第一讲第二节中所做的那样退出本教程： :q!
     或者，如果您可以访问另一个终端，请在那里执行以下操作。

  2. 在 shell 的提示符下输入命令： vim tutor <回车>
     'vim'是启动 Vim 编辑器的命令，'tutor'是您希望编辑的文件的名字。
     请使用一个可以改动的文件。

  3. 使用您在前面的教程中学到的命令插入删除文本。

  4. 保存改动过的文件并退出 Vim，按这些键： :wq  <回车>

  5. 如果您在步骤1中已经退出 vimtutor，请重启 vimtutor 移动到下面的小结一节。

  6. 阅读完以上步骤，弄懂它们的意义，然后在实践中进行练习。
```


**注意**
`:wq` 中的 `w` 是 `write`（写入）的缩写

## 第一讲小结

```zsh
  1. 光标在屏幕文本中的移动既可以用箭头键，也可以使用 hjkl 字母键。
         h (左移)       j (下行)       k (上行)     l (右移)

  2. 欲进入 Vim 编辑器(从命令行提示符)，请输入：vim 文件名 <回车>

  3. 欲退出 Vim 编辑器，请输入 <ESC>   :q!   <回车> 放弃所有改动。
                      或者输入 <ESC>   :wq   <回车> 保存改动。

  4. 在正常模式下删除光标所在位置的字符，请按： x

  5. 欲插入或添加文本，请输入：

         i   输入欲插入文本   <ESC>             在光标前插入文本
         A   输入欲添加文本   <ESC>             在一行后添加文本

特别提示：按下 <ESC> 键会带您回到正常模式或者撤消一个不想输入或部分完整
的命令。

好了，第一讲到此结束。下面接下来继续第二讲的内容。
```