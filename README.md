Download Link: https://assignmentchef.com/product/solved-cs204-advanced-programming-homework-7-inheritance-and-polymorphism
<br>
<h1>Introduction</h1>

<strong> </strong>In this homework, you are asked to implement a simple program using inheritance and polymorphism as described in the lectures. In this homework, you will be writing a base class called <strong>Human</strong> which is inherited by two classes: <strong>Muggle, Wizardkind.</strong> And <strong>Wizardkind</strong> class is also inherited by two other classes called: <strong>Student, GrownUp.</strong> The derived classes inherit the functions of their bases classes and also add new member variables and functions. The functions and variables the classes have is illustrated in the following diagram.




<h1>Class Definitions</h1>




<ul>

 <li>Human

  <ol>

   <li>Has two member variables: <strong>name</strong> and <strong>age</strong>.</li>

   <li>Has a function named: <strong>printInfo,</strong> which prints the name, age information of a human.</li>

  </ol></li>

 <li>Muggle

  <ol>

   <li>Has a member variable:</li>

   <li>Has <strong>printInfo</strong> function implemented to print <strong>job</strong> alongside name and age.</li>

  </ol></li>

 <li>Wizardkind

  <ol>

   <li>Has a member variable:</li>

   <li>Has <strong>printInfo</strong> function implemented to print <strong>wand</strong> alongside name and age.</li>

   <li>Has another function, called <strong>doSpell</strong> which takes a string parameter which is the spell to cast.</li>

  </ol></li>

 <li>Student

  <ol>

   <li>Has two more member variables: <strong>pet, houseName.</strong></li>

   <li>Has <strong>printInfo</strong> function implemented to print <strong>pet</strong> and <strong>houseName</strong> alongside name, age and wand.</li>

   <li>Has another function called <strong>feedPet</strong>, which prints a corresponding message.</li>

   <li>Examle: “Harry Potter fed Hedwig.”</li>

  </ol></li>

 <li>GrownUp

  <ol>

   <li>Has one additional member variable:</li>

   <li>Has <strong>printInfo</strong> function implemented to print <strong>job</strong> alongside name, age and wand.</li>

  </ol></li>

</ul>







<h1> Sample Main</h1>




You can use the main function provided below to test your program and compare the output of yours’ with the given output.




int main(){

Muggle vernon(“Vernon Dursley”, 50, “Director at Grunnings”);     vernon.printInfo();




cout &lt;&lt; endl;

Student Harry(“Harry Potter”, 16, “Phoenix Feather”, “Hedwig”, “Gryffindor”);        Harry.printInfo();




cout &lt;&lt; endl;

GrownUp Dumbledore(“Albus Dumbledore”, 110, “Elder Wand”, “Headmaster”);

Dumbledore.printInfo();




cout &lt;&lt; endl;

Dumbledore.doSpell(“Expecto Patronum”);




cout &lt;&lt; endl;

Harry.doSpell(“Expelliarmus”);




cout &lt;&lt; endl;        Harry.feedPet();




cout &lt;&lt; endl;

Student Ginny(“Ginny Weasley”, 15, “Yew wood”, “Arnold”, “Gryffindor”);

GrownUp Snape(“Severus Snape”, 35, “Dragon Heartstring”, “Potion Master”);

Student Hermione(“Hermione Granger”, 16, “Vine”, “Crookshanks”, “Gryffindor”);

Human hArray[6];




hArray[0] = vernon;        hArray[1] = Harry;      hArray[2] = Dumbledore;  hArray[3] = Ginny;  hArray[4] = Snape;

hArray[5] = Hermione;




Human * hPtr;        for (int i = 0; i &lt; 6; i++) {

cout &lt;&lt; endl;          hPtr = &amp;hArray[i];         hPtr-&gt;printInfo();

}




cout &lt;&lt; endl;

system(“pause”);




return 0;

}

<h1>Output</h1>




Muggle Informations

Name: Vernon Dursley

Age: 50

Job: Director at Grunnings




Student Wizardkind Informations

Name: Harry Potter

Age: 16

House: Gryffindor

Wand: Phoenix Feather

Pet: Hedwig




Grownup Wizardkind Informations

Name: Albus Dumbledore

Age: 110

Wand: Elder Wand

Job: Headmaster




Albus Dumbledore used spell: Expecto Patronum




Harry Potter used spell: Expelliarmus




Harry Potter fed Hedwig







Human informations

Name: Vernon Dursley

Age: 50







Human informations

Name: Harry Potter

Age: 16







Human informations

Name: Albus Dumbledore

Age: 110







Human informations

Name: Ginny Weasley

Age: 15







Human informations

Name: Severus Snape

Age: 35







Human informations

Name: Hermione Granger

Age: 16







Press any key to continue . . .







<h2>Some Important Rules</h2>

In order to get a full credit, your programs must be efficient and well presented, presence of any redundant computation or bad indentation, or missing, irrelevant comments are going to decrease your grades. You also have to use understandable identifier names, informative introduction and prompts. Modularity is also important; you have to use functions wherever needed and appropriate.




When we grade your homeworks we pay attention to these issues. Moreover, in order to observe the real performance of your codes, we are going to run your programs in <em>Release</em> mode and <strong>we may test your programs with very large test cases</strong>.




<strong> </strong>

<strong>What and where to submit (PLEASE READ, IMPORTANT) </strong>

You should prepare (or at least test) your program using MS Visual Studio 2012 C++. We will use the standard C++ compiler and libraries of the abovementioned platform while testing your homework. It’d be a good idea to write your name and last name in the program (as a comment line of course).




Submissions guidelines are below. Some parts of the grading process are automatic. Students are expected to strictly follow these guidelines in order to have a smooth grading process. If you do not follow these guidelines, depending on the severity of the problem created during the grading process, 5 or more penalty points are to be deducted from the grade. Name your cpp file that contains your program as follows:




<strong><em>“SUCourseUserName_YourLastname_YourName_HWnumber.cpp” </em></strong>




Your SUCourse user name is actually your SUNet username that is used for checking sabanciuniv e-mails. Do NOT use any spaces, non-ASCII and Turkish characters in the file name. For example, if your SUCourse user name is valent, name is Valentina, and last name is Tereşkova, then the file name must be:




<h2>Valent_Tereskova_Valentina_hw1.cpp</h2>




Do not add any other character or phrase to the file name. Make sure that this file is the latest version of your homework program. Compress this cpp file using WINZIP or WINRAR programs. Please use “zip” compression. “rar” or another compression mechanism is NOT allowed. Our homework processing system works only with zip files. Therefore, make sure that the resulting compressed file has a zip extension. Check that your compressed file opens up correctly and it contains your cpp file.




You will receive no credits if your compressed zip file does not expand or it does not contain the correct file. The naming convention of the zip file is the same as the cpp file (except the extension of the file of course). The name of the zip file should be as follows:




<strong><em>SUCourseUserName_YourLastname_YourName_HWnumber.zip </em></strong>




For example zubzipler_Zipleroglu_Zubeyir_hw1.zip is a valid name, but




<h2>hw1_hoz_HasanOz.zip, HasanOzHoz.zip</h2>




are <strong>NOT</strong> valid names.

<strong> </strong>

<strong>Submit via SUCourse ONLY!</strong> You will receive no credits if you submit by other means (email, paper, etc.).




Successful submission is one of the requirements of the homework. If, for some reason, you  cannot successfully submit your homework and we cannot grade it, your grade will be 0.

<strong> </strong>

Good Luck!

CS204 Team (M. Yusa Erguven, Kamer Kaya)

<strong> </strong>