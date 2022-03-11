---
layout: post
title:  "Print Current ViewController"
date:   2022-03-11 21:19:00 +0100
image: "../../../assets/print_current_view_controller.jpeg"
tags: breakpoint trick view-controller lldb
---

![](../../../assets/print_current_view_controller.jpeg)

<!--more-->

Add a symbolic breakpoint for the symbol `-[UIViewController viewDidAppear:]` and add a debugger
command of `po $arg1`. Make sure to activate the option "Automatically continue after evaluating
actions". When active, this breakpoint prints the name of the view controller that is currently
presenting the visible views. 
