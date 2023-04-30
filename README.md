Download Link: https://assignmentchef.com/product/solved-genghis-khents-students
<br>
<strong><u>What You Need to Do</u></strong>

You have some freedom on this assignment.

First, create a structure (named <em>Student</em>) that will describe each of Genghis Khent’s students. The structure contains the following member variables:

<ul>

 <li>An ID consisting of 4 digits. The data type should be a string or c-string instead of an int.</li>

 <li>A name, which may have embedded spaces (like “Genghis Khent”). The data type is a string or c-string.</li>

</ul>

Second, create a text file which lists students (say 25) in the format ID number, space, name. For example:

6666 Mini Me

2333 Help Me

7722 Yogi Beria

<strong>Note</strong>: There should be no duplicate IDs. However, so there will be some collisions, for about 12 of the 25 students, have 2 students have the same last 2 digits of the ID (e.g., no ID will duplicate, but the last 2 digits of the ID will).

Third, create a hash table class (using .h and .cpp files preferably) whose one member variable points to an array of 100 student structures. The placement of a student structure within the array is based on the last 2 digits of a student’s ID. Thus, a student with an ID ending in 45 will go in the 45th subscript ([45]) of the array, unless there’s a collision. The hash table class also would include the following member functions:

<em>Constructor</em> – Assigns to each element of the array the value NULL for the ID and the name. (Those values are how you determine if a slot is “empty”.

<em>Destructor</em> – If you’re using dynamic memory allocation. Otherwise probably not necessary.

<em>insert</em> – Has 2 parameters, representing ID and name, which are assigned to the member variables of the structure instance Assigns a student’s information (ID and name) to the proper element of the array. <strong>Important</strong>: Uses hashing to determine the proper array element, and resolves collisions.

<em>retrieve</em> – Has 1 parameter, the ID, and returns the student’s name, or NULL if no student with that ID exists. <strong>Important</strong>: Uses hashing to find that student in the array, and deals with collisions.

Fourth, create a driver or test file. This code will:

<ul>

 <li>Create an instance of the hash table class.</li>

 <li>Load the hash table from the text file, using the insert member</li>

 <li>Display a menu:

  <ul>

   <li>Find a student by ID. If chosen, the user is prompted to enter a 4 digit ID (no input validation necessary). Using the retrieve member                 function, the program either will output the name of the student                      associated with that ID, or report that no student has that ID.</li>

   <li>If chosen, the program will end.</li>

  </ul></li>

 <li></li>

</ul>


