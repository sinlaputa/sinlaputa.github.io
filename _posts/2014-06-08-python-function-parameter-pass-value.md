---
layout: post
title: "Python函数参数传递方式，对比C/C++/Java"
description: "说明python中函数参数方式，备忘"
tags: [python, function parameter]
modified: 2014-06-08
image:
  feature: abstract-1.jpg
##comments: true
##share: true
---

不同的程序设计语言函数参数的传递不一样，java与C++不同，之后的python又与前两者不同。对于先接触C/C++的程序员，python的函数传递方式并不具有自明性。

C/C++本身是静态语言，所有的变量都需要先声明后使用，对于一个新生成的对象，必须赋值给对应类型的值，否则会编译出错。对于函数参数的传递，按值传递、按引用传递需要明确指出（按指针传递只是按值传递的一种，只不过赋值的是指针本身的值，可以藉此修改指针指向的内容），不仅如此，类型也必须匹配才行。Java源于C++，保留了C++静态语言的模型，编译运行在JVM虚拟机上，离硬件更远相对来说更抽象（或者说更高级）。Java不在基于指针思考而是围绕着独享，所有的变量都是对对象的引用。值得注意的是，Java中有些类型的对象是不可变的，例如String类型，如要改变String变量的值，需要调用String对象的相关参数然后用返回值对String对象进行重新赋值。

## Cupidatat 90's lo-fi authentic try-hard

In pug Portland incididunt mlkshk put a bird on it vinyl quinoa. Terry Richardson shabby chic +1, scenester Tonx excepteur tempor fugiat voluptate fingerstache aliquip nisi next level. Farm-to-table hashtag Truffaut, Odd Future ex meggings gentrify single-origin coffee try-hard 90's. 

* Sartorial hoodie
* Labore viral forage
* Tote bag selvage
* DIY exercitation et id ugh tumblr church-key

Incididunt umami sriracha, ethical fugiat VHS ex assumenda yr irure direct trade. Marfa Truffaut bicycle rights, kitsch placeat Etsy kogi asymmetrical. Beard locavore flexitarian, kitsch photo booth hoodie plaid ethical readymade leggings yr.

Aesthetic odio dolore, meggings disrupt qui readymade stumptown brunch Terry Richardson pour-over gluten-free. Banksy american apparel in selfies, biodiesel flexitarian organic meh wolf quinoa gentrify banjo kogi. Readymade tofu ex, scenester dolor umami fingerstache occaecat fashion axe Carles jean shorts minim. Keffiyeh fashion axe nisi Godard mlkshk dolore. Lomo you probably haven't heard of them eu non, Odd Future Truffaut pug keytar meggings McSweeney's Pinterest cred. Etsy literally aute esse, eu bicycle rights qui meggings fanny pack. Gentrify leggings pug flannel duis.

## Forage occaecat cardigan qui

Fashion axe hella gastropub lo-fi kogi 90's aliquip +1 veniam delectus tousled. Cred sriracha locavore gastropub kale chips, iPhone mollit sartorial. Anim dolore 8-bit, pork belly dolor photo booth aute flannel small batch. Dolor disrupt ennui, tattooed whatever salvia Banksy sartorial roof party selfies raw denim sint meh pour-over. Ennui eu cardigan sint, gentrify iPhone cornhole. 

> Whatever velit occaecat quis deserunt gastropub, leggings elit tousled roof party 3 wolf moon kogi pug blue bottle ea. Fashion axe shabby chic Austin quinoa pickled laborum bitters next level, disrupt deep v accusamus non fingerstache.

