# ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE
___
## ___WELCOME TO ALX___

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQHmKf8fnlYjTTLoV2OxOln-ON52Uhb0IV7PQ&usqp=CAU" width="1500" height="250">

## MONTH 1

### ___EMACS GUIDE___
![Emacs](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT71Jprd_zomZAmZrqoJU32QaIK34NCzPwblA&usqp=CAU)
- [GNU Emacs](https://www.gnu.org/software/emacs/tour/)
- [Emacs Video Tutorial](https://www.youtube.com/watch?v=jPkIaqSh3cA)
- [Emacs From Scratch #1 - Getting Started with a Basic Usable Configuration](https://www.youtube.com/watch?v=74zOY-vgkyw)

___


### ___VIM GUIDE___
![Vim](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQls24qGIM1Sb2SpZm1hU6MK6hqobnenQlVf-f0yjFQfmzeXMjdeT-StuJBcVg5UkWdZWc&usqp=CAU)

- [Vim Editor Fundamentals](https://www.youtube.com/watch?v=XguBRi4TDNc)
- [Basic vi Commands](https://www.cs.colostate.edu/helpdocs/vi.html)

### Vi/Vim/Nvim keys and shortcuts
Coming from a click, touch, drag and drop world, command line tools and navigation might seem tricky at first. Don't fret. They are not difficult to learn, they are just not intuitive yet. As you use them daily, they will become a part of you.
Vi has two primary modes:
1. Command mode: Let's you execute commands like save, quit, formats, e.t.c.
2. Insert mode: When you type to populate a file.

To tell what mode you are in, watch the bottom left corner of your screen. Command mode displays nothing. Insert mode displays:
```
---INSERT---
```
When you open Vi, the default mode is the command mode. To start typing, press 'i' to enter into insert mode. Press ESC key to go back into command mode.

How to exit Vi:

You must be in command mode to execute these commands.

To quit an unedited document:
```
:q
```
To quit an edited document without saving changes:
```
:q!
```
To save progress without quitting
```
:w
```
To save and quit
```
:wq or :x
```
Other great commands:

- :set number - This command displays the numbering for each line. Makes it easy to trace mistakes and debug code.
- gg - Takes the cursor to the top of the file. Faster way to navigate than using arrow keys.
- dd - Deletes the entire line where the cursor is placed. Faster than delete or backspace button. Can also be used to paste the line elsewhere when you press 'p'.
- ?keyword - Used to search keywords in a document. For example, ?printf will look for all instances of 'printf'. If there are multiple instances, use 'n' and 'N' to jump between them forwards or backwards respectively.

How to debug code in the command line using vi:

1. Here's a simple code sample that prints a statement three times. Please note that this code was written specifically for demonstration purposes. The file name is saved as 'debug.c'

![0 program](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/421a96c1-8ea3-4184-9dd8-ed2898624a09)

2. When you run a betty check on the code, it gives you an error message. Notice the number '27' in front of the file name 'debug.c:27'. That number is the line number where the error occurred.

![1 error message](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/9c2f77fa-e5b0-4234-8943-a69df8d77396)

3. When you open the code in Vi again, type :set number and pressed Enter to display line numbers in the code. This makes it easy to track line 27.

![2  set number](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/3ade4971-7c1f-4560-b161-cd1de3b08ae4)

4. Two errors were flagged. "space prohibited before semicolon" and "void function return statements are not generally useful". For the sake of simplicity, I employed a basic fix.

![3 fix error](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/2f7e7b47-c039-452e-a56f-64bb5160dfbf)

5. Now when you run betty again, the code will be error free.

![4 error free](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/c41768ed-ca9d-443c-8809-24a95cfc8594)

6. To recap, check for the error line, read and understand the error message and address it accordingly. You can always ask your peers to help you interpret error messages that you don't yet understand. I hope this helps, however simplistic it might appear. Keep doing hard things!

![5 welcome](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/23355078/e9e66b73-1e19-4fa1-b96d-4c7e79aae524)

___


### ___SHELL, NAVIGATION___
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ01tiexbKmJEqe44i8xLb6ktAo0Otjj75HBg&usqp=CAU">

- [Video Tutorial on Shell Navigation](https://www.youtube.com/watch?v=UJ8n7Jz9HMc)
- [Shell Navigation Basics Part 1](http://linuxcommand.org/lc3_lts0020.php)
- [Shell Navigation Basics Part 2](http://linuxcommand.org/lc3_lts0030.php)
- [Manipulating Files](http://linuxcommand.org/lc3_lts0050.php)

___

### ___GIT AND GITHUB___
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRJ5r5PQ6gd9XnGlSu4LnBqV4lMDhZhQkKLiA&usqp=CAU">

- [Everything you need to know About GIT and GITHUB](https://www.youtube.com/watch?v=RGOj5yH7evk)
- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [About READMEs](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [How to Write a Git Commit Message](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes)
- [Git Branching](https://learngitbranching.js.org/)
- [Git Pull](https://codeinthehole.com/tips/pull-requests-and-other-good-practices-for-teams-using-github/)
- [Introduction to Version Control Systems | Git and Github for Beginners #1](https://www.youtube.com/watch?v=uxAsIobfu88)

___

### ___SHELL BASICS___
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTPTQoeA6Y9lv-vXeadtHRu-O1kX_6LYZi_Jw&usqp=CAU" >

#### ___From ALX Intranet___
- [What Is “The Shell”?](http://linuxcommand.org/lc3_lts0010.php)
- [Navigation](http://linuxcommand.org/lc3_lts0020.php)
- [Looking Around](http://linuxcommand.org/lc3_lts0030.php)
- [A Guided Tour](http://linuxcommand.org/lc3_lts0040.php)
- [Manipulating Files](http://linuxcommand.org/lc3_lts0050.php)
- [Working With Commands](http://linuxcommand.org/lc3_lts0060.php)
- [Reading Man pages](http://linuxcommand.org/lc3_man_pages/man1.html)
- [Keyboard shortcuts for Bash](https://www.howtogeek.com/181/keyboard-shortcuts-for-bash-command-shell-for-ubuntu-debian-suse-redhat-linux-etc/)
- [LTS](https://wiki.ubuntu.com/LTS)
- [Shebang](https://en.wikipedia.org/wiki/Shebang_%28Unix%29)

#### ___Personal Resourses___
- [Shell Scripting Tutorial for Beginners 1 - Introduction](https://www.youtube.com/watch?v=cQepf9fY6cE&list=PLS1QulWo1RIYmaxcEqw5JhK3b-6rgdWO_)
- [Shell For Absolute Beginners(Part 1)](https://www.youtube.com/watch?v=UJ8n7Jz9HMc&t=17s)
- [Shell For absolute Beginners. (Part 2 - basic commands)](https://www.youtube.com/watch?v=P8OP4kbIUKo&t=15s)

___

### ___SHELL PERMISSION___

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSS36E8aM5ThP0oGh5bvP2NelnmCcoeV_nJ_w&usqp=CAU">

#### ___From ALX Intranet___
- [Permissions](http://linuxcommand.org/lc3_lts0090.php)

#### ___Personal Resourses___
- [Linux File Permissions Cheat Sheet 1](https://www.stationx.net/linux-file-permissions-cheat-sheet/)
- [Linux File Permissions Cheat Sheet 2](https://www.psychz.net/client/kb/en/linux-file-permissions-cheat-sheet.html)

#### ___Videos Resourses___
- [Shell Permissions (CHMOD, CHGRP, CHOWN)](https://www.youtube.com/watch?v=vE5lXygsogg)
- [Unix Shell Scripting Tutorial](https://www.youtube.com/watch?v=HvonLym2eDw)
___

## ___Shell, init files, variables and expansions___

Expansions
Shell Arithmetic
Variables
Shell initialization files
The alias Command
Technical Writing



## ___C Programming___
<img width="300" height="150" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRo4GUjFkesFbctkKWs9GNPp1bjpZL-vLtLyg&usqp=CAU">

### ___Personal Resources___ 
- [C Programming](https://youtube.com/playlist?list=PL_c9BZzLwBRKKqOc9TJz1pP0ASrxLMtp2)
- [C programming: All you need to know.](https://youtube.com/playlist?list=PLdo5W4Nhv31a8UcMN9-35ghv8qyFWD9_S)
- [C Programming playlist](https://youtube.com/playlist?list=PL9ooVrP1hQOFrNo8jK9Yb2g2eMHz7hTu9)
<!-- ![Preprocessing Directives in C](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/117779858/cd641916-f29a-4250-b719-7f5cb78dac21) -->
- [Pre Processor Directives in C.](https://youtu.be/X6HiYbY3Uak)
<!-- ![compilation Process in C](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/117779858/84392048-50ff-4096-9f19-a491b1e50dfb) -->
- [Compiling and Linking in C.](https://youtu.be/HQAIj6ejefY)
<!-- ![pseudocodes and flowcharts](https://github.com/Innocentsax/ALX-RESOURCES_FROM_BEGINNER_TO_ADVANCE/assets/117779858/f4a42a16-ba48-4f04-88ab-30fc193876ad) -->
- [Pseudocode, flowchart, Algorithm and Whiteboarding.](https://youtu.be/cmqtfh-v13k)
- [All you need to know about static libraries.](https://dev.to/iamkhalil42/all-you-need-to-know-about-c-static-libraries-1o0b)
- [Difference between static and dynamic libraries.](https://www.linkedin.com/pulse/difference-between-static-vs-dynamic-libraries-nicolas-ribeiro/)
- [Varaiable functions](https://www.ibm.com/docs/en/ztpf/2021?topic=warnings-unused-variables-functions)
- [Understanding static libraries](https://www.linkedin.com/pulse/coding-ismo-playlist-understand-c-static-libraries-gil-posada)
- [Static libraries for beginners.](https://www.linkedin.com/pulse/c-static-libraries-beginners-mariem-matri/)
- [Nested loops](https://youtu.be/Bl21uAvRiXc)
- [Printf function](http://www.firmcodes.com/write-printf-function-c/)
- [Variadic function](https://youtu.be/S-ak715zIIE)
- [Printf project playlist](https://youtube.com/playlist?list=PL2yowC_WIiA5FUlIPz1XQceskxWT8pepB)
- [Learn different operators in C](https:/n/youtu.be/hOLAoo2p7gM)
- [Bit manipulations](https://codewise.hashnode.dev/) 


## ___Alx Resources___ 
### ___Hello World___

- [Everything you need to know to start with C pdf](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2022/4/e0ccf91eec6b977a9e00ed384dc285df9c2772e3.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230104%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230104T155404Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=dd33e8dfb92be3cc7150b3b9be22349b0be0a27502ad2e899c4191b9f0d1f902)
- [Hello world](https://youtu.be/co0b0xLEuRM)
- [Dennis Ritchie](https://en.wikipedia.org/wiki/Dennis_Ritchie)
- [“C” Programming Language: Brian Kernighan](https://youtu.be/de2Hsvxaf8M)
- [Why C programming is awesome](https://youtu.be/smGalmxPVYc)
- [Learning to program in C part 1](https://youtu.be/rk2fK2IIiiQ)
- [Learning to program in C part 2](https://youtu.be/FwpP_MsZWnU)
- [Understanding C compilation process](https://youtu.be/VDslRumKvRA)
- [Betting coding style](https://github.com/holbertonschool/Betty/wiki)
- [Hash-bang under the hood](https://twitter.com/unix_byte/status/1024147947393495040?s=21)
- [C vs C++](http://harmful.cat-v.org/software/c++/) 
- [Free Programming Tutorials](https://www.learninglad.com/)
___

### ___Variables, if, else, while___ 
- [Jenny Lectures](https://youtu.be/oWTnLzWkF5w)
- [Keywords and identifiers](https://publications.gbdirect.co.uk//c_book/chapter2/keywords_and_identifiers.html)
- [Integers](https://publications.gbdirect.co.uk//c_book/chapter2/integral_types.html)
- [Arithmetic Operators](https://www.tutorialspoint.com/cprogramming/c_arithmetic_operators.htm)
- [If statements in C](https://www.cprogramming.com/tutorial/c/lesson2.html)
- [If, else statements](https://www.tutorialspoint.com/cprogramming/if_else_statement_in_c.htm)
- [Relational Operation](https://www.tutorialspoint.com/cprogramming/c_relational_operators.htm)
- [Logical Operators](https://www.fresh2refresh.com/c-programming/c-operators-expressions/c-logical-operators/)
- [while Loop in C](https://www.tutorialspoint.com/cprogramming/c_while_loop.htm)

 ___Video Resouses___
- [While Loop](https://youtu.be/Ju1LYO9pkaI)

___

### ___Functions, nested loops___
- [C Functions](https://www.tutorialspoint.com/cprogramming/c_functions.htm)
- [What is the purpose of a function prototype](https://www.geeksforgeeks.org/what-is-the-purpose-of-a-function-prototype/)
- [C header files](https://www.tutorialspoint.com/cprogramming/c_header_files.htm)

__Video Resources___ 
- [Nested while loop](https://youtu.be/Z3iGeQ1gIss)
- [Learning to program in C](https://youtu.be/qMlnFwYdqIw)

___

### ___C Debugging___ 
- [Debugging](https://en.wikipedia.org/wiki/Debugging)
- [Rubber Duck debugging](https://www.thoughtfulcode.com/rubber-duck-debugging-psychology/)
___

### ___Pointers, arrays, and strings___ 
- [Pointer to pointer](https://www.tutorialspoint.com/cprogramming/c_pointer_to_pointer.htm)
- [Pointer to pointer with examples](https://beginnersbook.com/2014/01/c-pointer-to-pointer/)
- [Multi_dimentional arrays in C](https://www.tutorialspoint.com/cprogramming/c_multi_dimensional_arrays.htm)
- [Two-dimensional (2D) arrays in C programming with ](https://beginnersbook.com/2014/01/2d-arrays-in-c-example/)

___

### ___Recursion___ 
- [, introduction ](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/misc/2021/1/2818ba6f14f644b871dcbd746925fa15b8cd5937.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20230104%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230104T164913Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=97176d67e982b371ae5462ba88aba30c5362eb7f2c7956a953703d2378c290df)
- [Recursion for beginners](https://www.tutorialspoint.com/cprogramming/c_recursion.htm)

___Video Resources___ 
- [What on earth is recursion](https://youtu.be/Mv9NEXX1VHc)
- [Programming tutorials, recursion part 1](https://youtu.be/XGxbXMP6k8k)
- [Programming tutorials, recursion part 2](https://youtu.be/7XiIS6HobNs)



## Author
### **[UDO INNOCENT CHARLES](https://www.github.com/innocentsax)**, **[Owolabi Pius](https://www.github.com/opius2017)**


