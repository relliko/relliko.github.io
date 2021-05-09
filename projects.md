---
layout: page
title: "Projects"
permalink: /projects/
---
# fast-panopto
![fast-panopto layout](/images/fast-panopto.png)
<br>
<br>
fast-panopto is a small Chrome extension I wrote to enable users to select custom video player speeds for cases where they want to quickly go over a lecture or when the lecturer speaks slowly.
I only ever intended to use it personally but it ended up being more popular than I ever imagined with 2,500 weekly users at the time of writing this.

The chrome web store link can be found [here](https://chrome.google.com/webstore/detail/fast-panopto/bginlheikaacjjdajifcbakcmfcgmefh?hl=en) and the github page with a changelog is [here](https://github.com/relliko/fast-panopto).

# xk operating system
This project was huge and spanned the entire 11 weeks of the operating systems class I took at UW. We had to implement numerous system calls such as fork, exec, exit, fileopen, and fileread and others. I implemented a lot of kernel features that had to be built to work in a system where several processes could access shared data structures so utilizing mutex locks was essential. It was also necessary to manage memory perfectly. Particularly when working with memory paging for a process, things had to be perfect or there would obviously be massive problems when a process is being forked and trying to execute. Naturally, working in such a sensitive system required in-depth debugging so I became comfortable using GDB and Valgrind to debug along with test code to check edge cases. There was a lot of other features such as copy-on-write forking and filesystem details like file descriptors and write-ahead logging to ensure crash safety on the disk. My partner and I chose to implement interprocess communication using signals as a bonus feature at the end of the course. 