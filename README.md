https://sikandss.github.io/Cross-Platform-Excel-Clone/

#Copy pasted my personal notes on here so the description wont make much sense without the formatting.




Excel clone
Beginning stage


Made a rough UI design using freeware software on the interwebs. Define all content relationship and follow up with a slight dive into the DOM tree.
 
 
To prevent content from running all over the place It’s a good practice to establish the design direction first.

 Expanding the UI design by adding the functionalities envisioned and expanding the UI design.

 





Skeleton Code
Now that we’ve established the basic DOM structure. We write the skeleton code.
HTML 
 

CSS
•	Vh: viewport-height
Ex: 50 vh uses 50% of broswer’s display screen
•	Box-sizing: border-box
So the divs only use up the specified value of space and include borders with the 50vh space allocated to it. Now the padding and border is included in 50vh.


 
Margin : 0 to remove all margins 
Overflow : hidden to remove scroll wheels
Font-size 14; 14 size font throughout
 
Box-sizing: border-box to remove the padding and border automatically taking extra space.
  
Giving all skeleton div tags height and borders to check out how the skeleton format looks.
Title Bar
 
HTML
 
CSS
 
height : 5vh; gives 5% of viewport height
background-color :  #12f233f3; gives color to the background 
display : flex; applies flexbox to the div tag.
Justify-content : center; horizontally align if flex direction is row
Align-tems: center;vertically align if flex direction vertical
Color : #fff; colors the inside text white




MENU BAR
 
HTML
 
CSS
 
•	Padding-left : 10px; gives 10 px space from div boundary inside.
•	Padding-right : 10px; gives 10 px space from div doundary      inside.
•	Cursor : pointer;
•	Cursor : default; changes pointer on hover
•	.class:hover {
} changes div properties when hovering over it



















MENU ICON BAR
 
 
html
 
 
Css
 

Font-family : “Noto Sans”; gives select tag a font 





How to get the menu-icons
 
 
Link the html with google icon api:
 

Use the google api in divs:
Content_cut for  
Content_copy for  
And so on………
 

 









Formula Bar
 
Html
 
Css
 
Padding here took care of the formula editor not touching the border.
 
 
  has both classes formula editor and selected cell which makes it 120 px wide.
 



DATA CONTAINER
HTML
 
Css
 
Flex-wrap : wrap; Use wrap for wrapping the div tags around
 

 
 
 
 
 
 
 




Sheet Bar
 
 
Html
 
CSS
 
 
 
 
 





Functionalities 
ROW AND COLUMN COUNT
 
 







Cell Grid
 
 











Multiple cell select
 
 
 

















Multiple select of Bold, Underlined and Italics.  
 
We just need to toggle the selected class in this case as the Bold, Italics and Underlined properties can all be present for a text or a mixture of those.
Select of Align-items
 
 
We remove the selected class from whoever that has it and give it to the clicked align button.
Select input cell
 
 
We remove the selected class from whichever cell was being typed in and add selected class to the new cell that is being typed in.
Scrolling 
 

Add and event listener and add the scroll action with this.scrollLeft/Right









Update Cell properties
 
 
 

 





Header change of selected options when selecting other input cells
 
















Defining sheets
Default sheet properties
 
 .
 


