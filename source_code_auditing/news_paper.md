# News Paper Walkthrough

When given a relatively large application, it is important not to get lost in the code itself because there is a lot of information you can gather without digging into the nitty gritty details of the program. It helps to have a general approach when auditing something like this to be as efficient as possible.

## Step 1 - Play with it
A good first step is to use the application the way it was meant to be used. Getting an idea as to what functionaity the user has access to will help you later when you are brainstorming possible vulnerabilities.

## Step 2 - Scan for keywords
After you have a feel for how the program works, we will want to glance at the code for any comments, variables and functions that are interesting. We may be looking for a comment that has a username and password or a function that gives us root access to the computer. Stuff like this is a very big asset for a later exploit we might develop as we could use this code to our advantage.

## Step 3 - Bad programming
At this point we want to really look at the code itself to identify functions that really should not be used because they have been declared vulnerable or coding practices that could cause a bug to occur. Knowing the language the program is in is crucial to understanding potential flaws

## Step 4 - Crash it!
Once we have some flaws identified, we should try to make the program crash. It may seem silly to want to crash the program, but being able to crash it means we can make the program behave unexpectedly. Now once the program is operating unexpectedly, we have now out-smarted the programmer because he obviously doesn't want his program to crash, but *we* can make it! 

## Next Steps - Exploitation
Now that we have some known flaw in the program and we can make it behave unexpectedly, we can now try to control the flow of execution of the program and essentially add our own functionality to the program to make it do our bidding, this is known as exploitation.
