# Week 3 - Source Code Auditing \\\\ Part 2
This week we will continue with the final video on Code Auditing, and provide you with 2 more applications that are intentionally vulnerable. Your job is to audit the source code and find vulnerabilities in them. Test
the skills that you have learned last week to efficiently go over the process of auditing applications.

### Lecture Materials
1. [Code Auditing 101](http://vimeo.com/30001189/) [[slides](https://github.com/isislab/Hack-Night/blob/master/2014-Fall/slides/code_audits_1_fall2011.pdf?raw=true)]
2. [Code Auditing 102](http://vimeo.com/29702192/) [[slides](https://github.com/isislab/Hack-Night/blob/master/2014-Fall/slides/code_audits_2_fall2011.pdf?raw=true)]

### Workshop Materials
#### What we will be covering
1. [Memory Corruption Examples]( https://github.com/isislab/Hack-Night/tree/master/2015-Spring/workshops/week3/memory_corruption)
2. https://picoctf.com/binary_demo/binary_demo.html#1
3. 

#### Material we might cover
1. [News Paper](https://github.com/isislab/Hack-Night/blob/master/2014-Fall/workshops/week3/news_server.c):
This network service simulates a text-based terminal application. The general purpose of the application is to act as a "news server" or text file service. These are two types of users: regular and administrator. Administrators can add users and execute back-end system commands. Users can view and contribute articles (aka text files). Assume the application runs on Linux and is compiled with gcc. ([Simple Usage](https://github.com/isislab/Hack-Night/blob/master/2014-Fall/workshops/week3/news_install.sh))
2. [Siberia Crimeware Pack](https://github.com/isislab/Hack-Night/blob/master/2014-Fall/workshops/week3/siberia.zip?raw=true): (Password: infected)
The Siberia kit contains live exploit code and will likely set off AV, however none of the exploit code is in a state where it would be harmful to your computer. In addition to all of the vulnerabilites have been patched years ago, the exploits in Siberia need to be interpreted by PHP and read by your browser for them to have any effect. You can safely disable or create exceptions in your AV for this exercise or place the Siberia files inside a VM.

### Resources
1. [Source Code Analysis](https://github.com/isislab/Project-Ideas/wiki/Source-Code-Analysis)
2. [Application Security](https://github.com/isislab/Project-Ideas/wiki/Application-Security)
3. [The Art of Software Security Assessment](http://www.amazon.com/Art-Software-Security-Assessment-Vulnerabilities/dp/0321444426/ref=sr_1_1?s=books&ie=UTF8&qid=1367449909&sr=1-1&keywords=the+art+of+software+security+assessment)
4. [Integer Overflows](http://en.wikipedia.org/wiki/Integer_overflow)
5. [Catching Integer Overflows](http://www.fefe.de/intof.html)
6. [The Fortify Taxonomy of Software Security Flaws](http://www.fortify.com/vulncat/)

### Tools
1. [Source Navigator](http://sourcenav.sourceforge.net/)
2. [Scitools Understand](http://www.scitools.com/)
3. [List of tools for static code analysis](http://en.wikipedia.org/wiki/List_of_tools_for_static_code_analysis)
