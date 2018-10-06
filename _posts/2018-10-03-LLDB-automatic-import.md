---
layout: post
title: LLDB automatically import UIKit inside Xcode 
---

It turns out that the easiest way to automatically import UIKit, or any other framework, inside Xcodes LLDB is to create a breakpoint that will execute the debbugers command. Go to the main function and create a new breakpoint. Then edit the breakpoint and attach `e @import UIKit` statement as debugger command. Also, be sure to select Automatically continue after evaluating actions.

![_config.yml]({{ site.baseurl }}/images/breakpoint_debugger_command.png)
