## History of Linux and Unix

- we cand divided into three stages:

  1. from 1964 to 1984

     - in 1964 three foundations (General Electric$$$(funding foundation and company), bellabs(AT&T researching foundation)and MIT(educational foundation)) agreed on making time sharing operating system, before 1964 os was called syrup processing system which means that a user is processing something and another user has to wait till the first user finishes all the his tasks and then the second user starts his tasks, tasks are executed one by one till before the next task.
     - the three foundation succeded in 1965 to make an operating system and in 1968-69 was completely developed and called Multics , this operating system allowed multi users to connect on the same machine with same hardware and run many tasks in the same time. but the project didn't make the goals defined and two foundation withdrew their support GE and MIT.
     - Bellabs continued to develop Multics till 1970 and introduce Uincs written with B language and fortran language, and a new release was introduced in 1971 written with C language with the name unix and in 1972 and 1973 new versions of unix appeared.
     - Bellabs wanted to make their operating system usable and famous so they targetted university student by sending their scientist to train them on the new operating system and gave them free copy of the operating system. In Berkely university in 1976 the students wrote and developed some apps that works on that operating system and they added TCP/IP stack to unix and they created editors like Ed and Joe. and they decided to call their new version BSD short name for Berkly software distribution.
     - Bellab got angry about that and decided to ban the free copy distribution and force a licensed copy so anyone uses it has to refer Bellab to save their rights. Bellab sold a license to IBM to use it for commerical use and they made their version called AIX, HP bought it and made HP unix, Apple made MACosx,
       and Sun mad Solaris. Many versions appeared and it become a product for selling and buying
     - The Bellabs scientist didn't like what Bellabs management did and they left the company and decided to make another operation system for a free license to prevent Bellabs Monopoly. Richard Stallman (what an activist) was one of the original scientist who developed unix. He wanted a free use of the operating system so that anyone can use, he started in late 1983 and begining of 1984.

  2. from 1984 to 1991

     - an operating system components are , Kernal which is the core of the operating system it is software component not physical component that talks with the hardware the physical component and command it execute commands to the sound card, memory , hard disk and other hardware devices in other words it makes the command and the processor makes this command into instructions so the other hardware can perform these instructions. any command is transfered into 0 and 1 and the kernal takes them, operate on them and send them to the hardware to execute the command.
     - The kernal needs libraries,compiler and shell which is the layer above the kernal and applications and GUI which are another layer above the libraries.

     - Richard Stallman started on developing the free operating system called GNU which stands for 'GNU Not Unix', Note that free means that the source code is free to be developed by others and compiled for use.
     - He only made applications,libraries, shell and a compiler called GCC 'GNU C Compiler' that allows to write code and transfer it into a binary or application but he coudn't make a kernal.
     - That was in the seven years in this stage and he did all that with the help of other developers and programmers.
     - Note that Richard depended on the BSD version developed and released by Berkely students before Bellab made a license for Unix and BSD is now still existing with other variants like OpenBSD and FreeBSD an d NETBSD Note also that The BSD is the Backbone for DNS of the whole internet.

  3. from 1991 to till now

     - in 1991, one of Richard students called linus torvalds made a kernal that supports hard disks with only type AT and supports multi threading or multi tasking which means that an app can be paused and another app can work and the paused app can be resumed after the second app is paused and that is different from previous operating system that allows an app to work till it completely finishes it task and then next app can work.
     - Linus talked about this work in a message and Richard noticed this message and he sensed that something new is in the air. to complete his operating system. He communicated with linus and asked him to use his kernal to complete his operating system and he asked him to name the kernal. Linus is from finland and seeing a Tux in the snow and getting beaten by one inspired him to call the kernal LINUX and the operating system GNU LINUX but now it is famously known as LINUX.
     - in 1993 was real starting for stage 3 as two projects appeared Slackware and Debian.
     - Slackware took the apps of GNU and the shell and libraries and kernal and made slackware linux also Debian made the same and called it Debian linux.
     - NOTE THAT GNE code is free and GNu made a FSF stands for free software foundation this foundation has a target to keep the free code always free so if some company A used a free code from another B so the company has to release the new code for free and also made GPL general public license which give the right to sell the application of company A but their source code is always free and belongs to the original owner of the original code company B as company B released the code with GPL(general public licence) and FSF is about saving the rights for the original owner. so, releasing a source code has to be with GPL. FSF is about keeping the code free.
     - so registering your code under GPL saves your rights as an original creator to the code. and if added new code people should be aware of this new code and don't waste their time to redo it again
     - in 1994, Redhat company appeared and did the same but what is the different between slackware Debian and Redhat ? all have the most of the same packages they only differs in few packages that each company saw that the implementation of these different packages works best for them.
     - in 1988, redhat realesed till version 9 called redhat linux after that they stopped that and they released two versions one for the home users , developers and testers called fedora and the other is called redhat enterprise linux for enterprise world
     - redhat kept the source code free you can take and build it yourself but the application and they build you pay for it to take the support and the updates. normally they give 10 years and you can request special extended support for 12 years and this is for the enterprise version
     - for fedora the release life time is 4 to 6 months and the enterprise release life time is more than 24 month as they say but in real life they release a new version every 4 to 5 years. in fedora new features and applicatins are introduced and used by the users for trial once they become stable with no issues redhats moves these applications to the enterprise version.
     - as fedora redhat is full of bugs , students can't afford buying the enterprise version of redhat so they took the enterprise source code and compile and build it under the name of centos which means cent for the OS.
     - there are three companys in the market, redhat , suse and debian , suse has SLES (suse linux enterprise servers) and open suse which is the same concept as fedora , new features in open suse and once they become stable they move to SLES.
     - Debian is very stable as redhat , but Debian doesn't has commercial support like redhat and suse
     - ubunto is an implementation based on Debian and fedora is based on redhat
     - SL scientific linux is based on redhat enterprise and Helios is based on SL, Helios is used in medical institutes and health care IT.
     - note that in 1984 to 91 , they developed the apps on Unix and when the linux kernal appeared they moved the apps to GNU linux and that shows the relation between Unix and linux
     - note that linus the guy who made the kernal has developed it on minix which is a free updated version on Unix.
