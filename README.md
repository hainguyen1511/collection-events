# Collection Events
* A program to create a collection of all of the events, celebrities,
* Fan favorites you want to participate in if you were going to the next Comic Con.

> [!IMPORTANT]
> Implement the functionality in this order:
Task 1. Create the structure and allow the user to add a new event,
celebrity, fan favorite. Place each new item in an array of structures.
Task 2. Save the current list of events, celebrities, and fan favorites to the
external file
Task 3. Display all items
Task 4. Load items from the file previously stored (until array is full)
Task 5. Provide a menu interface to allow the user to select from (a) adding
a new item, (b) displaying all, (c) loading from a file, or (d) quit.
Task 6. Display all item that match a particular event’s name

> [!TIP]
> Step 1. Set up the preprocessor directives for programming. This time we have to #include <fstream>.
Also, remember to set up struct like the global variables.

> [!TIP]
> Step 2. Set up the prototypes.
There are 9 functions call I can think of that is essential for program 3.
a.	The void function to print out the welcome message.
b.	The integer function returns the integer from the select option.
c.	The void function to get event details.
d.	The void function loads but then have to modify the number of numbers loaded.
e.	The function to write to external files.
f.	The void function displays everything in arrays of structs
g.	And a matching function to look for matching events.

> [!TIP]
> Step 3. Set up the main function.
The main function will contain the constant for the size of arrays of the struct. We also declare the struct here to pass the arrays of the struct to other functions. We also have several events here to pass by reference. Then setting up the if and else if statements for all of the options after we have the returned value from the function option.

> [!TIP]
> Step 4. Set up the welcome function.
Not a lot here but making sure to welcome the user and show the purpose of the program.

> [!TIP]
> Step 5. Set up the option function. This will print out all menu options:
1. Enter a new event, celebrity, fan favorite 
2. Display a match of a particular event, celebrity, fan favorite 
3. Display all 
4. Save all items to an external data file 
5. Load from an external data file 
Also, I will add a caution for the user to understand that they have to load the external file manually to add to the previous list. Else, this program will erase everything in the external file and we start from the beginning. Make sure we have a cin.ignore here.

> [!TIP]
> Step 6. Setup function to get detail of events. I make sure to pass the arrays of structs, number of events by reference, and count by reference. Set up a for loops to get input up to 10 stacks of arrays. Loops will be done when reply n.

> [!TIP]
> Step 7. Function to load info from an external file. I declare the ifstreamfile_in then I type the code to open the file name "comic_con.txt". If opening a file is successful, a while loop will be looping and it is going to load until the end of a file, and the if statement file_in.eof(). Use file_in.get like the 3 arguments of cin.get for each member of structs, and file_in.ignore. I need to remember to close out the file.

> [!TIP]
> Step 8. Set up the function to write to the external file. I call the stream file_out. I make sure to save the file as comic_con.txt. I also print out with loops the arrays of structs. Then close out the file. I need to remember the file_out  << list[i]. members code to successfully execute the printout to file successfully.

> [!TIP]
> Step 9. Print out the display function. This is an easy function with a while loop that then passes the arrays of each member of structs in and keeps printing until reaches the number of events which has been loaded.

> [!TIP]
> Step 10. Make a void function for getting input to match with a word in an external file. This function also makes a call to the special function which is going to use the strcmp to match with the user input.

> [!TIP]
> Step 11. Set up a function to show the matching event. It should receive a modified value from the matching function. Then specify the print stamen to the matching item-value-integer.

> [!TIP]
> Step 12. Finally, we reorganize the main function. Option 1 is to get detail. Option 2 is to call the function for matching. Option 3 is for calling to display everything in the input stream. Option 4 is for saving the events to the file. Option 5 is for loading up details from an external file. Other options or bad input will make the program quits.
