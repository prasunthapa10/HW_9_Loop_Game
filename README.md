# HW_9_Loop_Game 
# Addition Game 
# Introduction
We are going to customize our addition game code using the methods and loops. This helps to make our code
shorter and more effective.

# Project Outline
```
//Call the addition game method.
// Assign the value for hardness, score and hardness setup.
// Set up my for loop to go through the number of rounds
//  Use the boolean data type to verify the answer
// Use the if statement to compare the answers and Print statement to print the result.
```
##  References & Literature
*   Liang, Y. (2014). *Introduction to Java programming: Comprehensive version* (Tenth ed.).

## Source Code
```java
 @author LAB
 *
 */import java.util.Scanner;
public class Loop_Game {

	/**
	 * @param args
	 */
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println("Hello Team.");
		//Call the addition game method.
		AdditonGameMethod();
		}
		public static void AdditonGameMethod() {
		System.out.println("Inside the addition game method.");
		// Assign the value for hardness, score and hardness setup.
		int hardness = 10;
		int hardnessStep = 10;
		int score = 0;
		// Set up my for loop to go through the number of rounds
		int numberOfRounds = 4;
		for(int roundNumber = 1;
		roundNumber <= numberOfRounds;
		roundNumber = roundNumber + 1){
		System.out.println("Inside the for loop. Round: " + roundNumber);
		// Using the boolean data type to verify the answer
		boolean isAnswerCorrect = getAndCheckStudentAnswer(hardness);
		if(isAnswerCorrect){
		System.out.print("Your score was " + score + " and is now ");
		score = score + hardness;
		System.out.println(score + ".");
		if(roundNumber<numberOfRounds){
		System.out.print("Your hardness was " + hardness + " and is now ");
		hardness = hardness * hardnessStep;
		System.out.println(hardness + ".");
		}
		}else{
		if(roundNumber<numberOfRounds){
		System.out.print("Your hardness was " + hardness + " and is now ");
		if(hardness>10){
		hardness = hardness / hardnessStep;
		}
		System.out.println(hardness + ".");
		}
		}
		}
		System.out.println("The game is complete.");
		System.out.println("Your final score was " + score );
		}
		public static boolean getAndCheckStudentAnswer(int hardness) {
		System.out.println("Inside get and check student answer method.");
		int number1 = (int)(Math.random()*hardness);
		int number2 = (int)(Math.random()*hardness);
		System.out.println("Add " + number1 + " and " + number2 +".");
		//Scanner input = new Scanner(System.in);
		//int studentAnswer = input.nextInt();
		Scanner get = new Scanner(System.in);
		int studentAnswer = get.nextInt();
		if(studentAnswer == (number1 + number2)){
		System.out.println("Good work, your answer was correct.");
		return true;
		}else{
		System.out.println("Nice try, but the correct answer was " + (number1 + number2));
		return false;
		}

	
}
	}
	
```
	


## Console Output
```

Hello Team.
Inside the addition game method.
Inside the for loop. Round: 1
Inside get and check student answer method.
Add 1 and 1.
2
Good work, your answer was correct.
Your score was 0 and is now 10.
Your hardness was 10 and is now 100.
Inside the for loop. Round: 2
Inside get and check student answer method.
Add 91 and 85.
100
Nice try, but the correct answer was 176
Your hardness was 100 and is now 10.
Inside the for loop. Round: 3
Inside get and check student answer method.
Add 4 and 5.
9
Good work, your answer was correct.
Your score was 10 and is now 20.
Your hardness was 10 and is now 100.
Inside the for loop. Round: 4
Inside get and check student answer method.
Add 94 and 81.
322
Nice try, but the correct answer was 175
The game is complete.
Your final score was 20
```


# Command Prompt
```


E:\>Dir
 Volume in drive E is PRASUN
 Volume Serial Number is B0CF-9DF4

 Directory of E:\

10/09/2015  10:22 AM    <DIR>          .metadata
10/09/2015  10:22 AM    <DIR>          Prasun
10/26/2015  10:05 AM        12,563,873 introduction-to-java-programming-comprehe
nsive-version-10th-edition.zip
10/26/2015  10:13 AM    <DIR>          Fun_With_Functions
10/26/2015  10:42 AM             2,706 Comment_Line_md.txt
11/02/2015  10:30 AM    <DIR>          Listing_Project
11/03/2015  10:07 PM             3,394 Command.txt
02/11/2015  11:05 PM    <DIR>          workspace
11/04/2015  04:27 PM             9,982 README.md
11/11/2015  10:38 AM    <DIR>          Methods_Loops_Addition_Game
               4 File(s)     12,579,955 bytes
               6 Dir(s)  15,405,072,384 bytes free

E:\>cd Methods_Loops_Addition_Game

E:\Methods_Loops_Addition_Game>echo # HW_9_Loop_Game >> README.md

E:\Methods_Loops_Addition_Game>git init
Initialized empty Git repository in E:/Methods_Loops_Addition_Game/.git/

E:\Methods_Loops_Addition_Game>git add README.md

E:\Methods_Loops_Addition_Game>git config user.name "Prasun Thapa"

E:\Methods_Loops_Addition_Game>git config user.email thapap@student.swosu.edu

E:\Methods_Loops_Addition_Game>git commit -m "First commit"
[master (root-commit) 6f92b53] First commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

E:\Methods_Loops_Addition_Game>git remote add origin https://github.com/prasunth
apa10/HW_9_Loop_Game.git

E:\Methods_Loops_Addition_Game>git push -u origin master
Username for 'https://github.com': prasunthapa10
Password for 'https://prasunthapa10@github.com':
Counting objects: 3, done.
Writing objects: 100% (3/3), 238 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/prasunthapa10/HW_9_Loop_Game.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.

E:\Methods_Loops_Addition_Game>git add .

E:\Methods_Loops_Addition_Game>git commit -m "Some codes"
[master 5f8e2d3] Some codes
 4 files changed, 96 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 bin/Loop_Game.class
 create mode 100644 src/Loop_Game.java

E:\Methods_Loops_Addition_Game>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Username for 'https://github.com': prasunthapa10
Password for 'https://prasunthapa10@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (8/8), 2.83 KiB | 0 bytes/s, done.
Total 8 (delta 0), reused 0 (delta 0)
To https://github.com/prasunthapa10/HW_9_Loop_Game.git
   6f92b53..5f8e2d3  master -> master

E:\Methods_Loops_Addition_Game>
```
## Summary
From this source code we can easily figure out how the methods have made our life easier. We have also used the for loop that has helped to generate the same loop for four times. The pevious addition gam without loops and methods was too long, but now the code has become short and sweet. Instead of typing the same code for four rounds, we used the for loop. We use the public static void method and public static boolean method to make our code easier in the above program. We can use the same concept to find the otput of other programs in the upcoming days.  
