# Cocktail-Sort-Visualizer
This Project is consisting of HTML, CSS, JavaScript and jQuery. With the help of VS Code, I have implemented all components.

HTML Components Used:
1.	Head Tag:
•	Title Tag- Containing name of title of web Page “Cocktail Sort Visualizer”.
2.	Body Tag- Containing all other Tags.
3.	Heading Tag:
•	Heading 1- This is for Showing this Project is Cocktail Sort Visualizer.
•	Heading 2- This for asking user for numbers.
4.	Input Tag:
•	Textbox- This is for taking input from user as number.
5.	Span Tag: 
•	Span 1- To print the Array Entered by user.
•	Span 2- To show status of sorting and print the Sorted Array.
6.	Paragraph Tag- To separate the tags by making space with empty paragraph.
7.	Button Tag:
•	Button 1- This is “Submit Button” to print the array entered by user in Textbox.
•	Button 2- This is “Clear Button” to remove all value entered by user and clear bars.
•	Button 3- This is “Generate Bars” Button to generate Vertical bars according to entered array values.
•	Button 4- This is “Sort It” Button to sort the bars using Cocktail Sort method.
8.	Div. Tag- This is Container to put Vertical Bars corresponding to each value one by one.
9.	Link Tag:
•	Link Tag 1-To link CSS file in the document inside Head Tag.
•	Link Tag 2-To link JavaScript file in the document inside HTML Tag.
•	Link Tag 3-To link jQuery Library in the document inside HTML Tag.

CSS Components Used:
1.	Body:
•	Background Color, Font family
2.	Heading 1: 
•	Margin, Text Alignment, Font Size, Background Color, Color
•	Border-radius, Font-weight
3.	Heading 2:
•	Margin, Width, Padding, Text Alignment, Font Size, Background Color
•	Color, Border-radius, Font-weight
4.	Textbox:
•	Height and width, Border, Border radius, Font size, Font family
•	Padding, Font weight
5.	Container:
•	Height, Position, Margin-top, Align-content
6.	Bars 
•	Width, position, align-self, background-color, transition, border-radius
7.	Bars Id
•	Position, Text alignment, width, color
8.	Buttons:
•	Padding, font-weight, Border-radius, Background-color
•	Font-size, Border, Color

JavaScript Components Used:
1.	querySelector:
•	To work on container of bars and bars.
2.	getElementById:
•	To work on textbox, and all Buttons
3.	Function 1: “input”
•	To validate the user entering value or not
•	If user start Typing in textbox, then only submit button will get enable otherwise disabled.
•	Hover effect with help of jQuery will work when the buttons are enabled otherwise hover effect will not work.
4.	Function 2: “generatearray”
•	It will convert value entered in textbox into array with help of splitted values to split the value of textbox.
•	When user enter the value in textbox, then on clicking submit button function will check that all number should be upto 100 only. If any number is greater than 100 then page will give alert. If numbers are correct, it proceeds further.
•	This function will also check whether array is already sorted or not.
•	If array is already sorted, then it will print “Given Array is already sorted” otherwise it will print the entered array and then “clear” button will get enable and “Submit” button will get disable.
•	It will also show styling in text printed above with help of jQuery.
•	After printing array, it will enable the “Generate Bars” Button.
5.	Function 3: “generatebars” function -
•	On clicking Button “Generate Bars” this function will work.
•	This function will disable the Generate Bars and button color will also get change.
•	There is a “for loop” to generate Bar corresponding to that value in terms of height and width. Bars will get added one by one in the container by creating div element for each bar. Each bar generates after some interval with help of await function.
•	After bar generation “Sort it” button will get enable.
6.	Function 4: “Sorting” 
•	This function will show Sorting status below the container.
•	I have also applied some CSS properties using jQuery to show sorting status.
7.	Function 5: “Cocktail Sort” function is asynchronous function-
•	Asynchronous function provides await function to pause the execution of code for some time interval. This function will sort the bars with some interval with help of await function. 
•	It will firstly sort from left to right and then right to left till sorting completion.
•	For Sorting it will select two bars at a time and will compare their values and it will swap the smaller value from larger value to left direction.
•	This comparing and swapping will repeat from both side till sorted, there will be some interval between comparing and swapping the values and bars.
•	Different colors are used to indicate which elements are unsorted(sky-blue), compared(red) & sorted (light green).
8.	 For retrieving sorted array
•	Finally, we will get alert “Sorting status as Completed” and will print the sorted array below the container.
9.	Function 6: “removevalues”
•	This function will clear all values and sorting results.
•	It will simply reload the tab.

