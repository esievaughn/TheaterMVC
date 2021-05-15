# TheaterMVC

#### OVERVIEW
For the C# Live Project, I worked a one week sprint on scrum team developing a web application utilizing ASP.NET Entity Framework for a Theater in Portland. The team worked through Azure following scrum/agile methodologies, and used slack and google meet for communication. I worked on building the Rental History section of the website with CRUD functionality. 


#### Story #1: Style Contact Page
Tasked with stylizing the website's main Contact page based on UI/UX standards already set for the project. 

- [CONTACT PAGE: UI/UX standards](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/contactPg.png)

![](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/csscontactpage.png)



#### Story #2: Create entity model for Rental History and CRUD pages

I created a model based on the schema given which mapped to to a new database, giving the RentalHistoryID the "ID" thereby assiging it as the primary key. Using code first, I created the database. I then scaffoled a RentalHistory controller and CRUD pages for the RentalHistory model. This created Index, Create, Details, Delete and Edit pages. Then tested the CRUD functionality ensuring users could navigate to each page by typing in the address of the page in the URL, and that that RentalHistory could be created, edited, and deleted successfully.

- [RENTAL HISTORY MODEL](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/rentalhistoryModel.png)

![](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/models.png)



#### Story #3: Rental History Create & Edit Pages
The next story focused on styling the Create and Edit pages with given parameters. I rearranged the RentalDamaged label and checkbox to be on the same line.  Restricted the form's width to a maximum of around 600 pixels.  Brought the Back to List button into the form and center both the Back to List button and Create button. Then, I created a jquery script to change the checkbox if a Rental is not damaged from the "DamagesIncurred property" to "Notes" instead. I utilized the on ready function so that the Edit page would loved either the "DamagesIncurred property" or "Notes" label depending on what the user saved. I passed in parameters to the jQuery script by adding classes to the Razer HTMl helpers. 

- [CREATE PAGE](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/createCrud.png)
- [EDIT PAGE](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/editCrud.png)
![](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/stylingcrud.gif)

#### Story #4: Rental History Index Page
Styled the index page to show all of the Rental Histories in tabular form. If a Rental is damaged, added a red X on the left side of that cell. And if the Rental is not damaged, added a be a green checkmark. Under a Razor foreach statement, I implemented a Razor if statement with the red X and greencheckmark to properly display the image based on what the user saved for rental damaged. After the X or checkmark symbol, the name of the Rental is displayed and styled so the text so that is distinguished from the other text in the cell using a Bootstrap badge.After the Rental name, Damages Incurred text is displayed.  If the Rental is not damaged, the text is greyed out, set to no wrap with an ellipses to cut off the text. To gray out the text for the Rentals that are not damaged, I utilized anoter Razor if statement based on the Rental Damaged property. Finally, when hovering over a cell, a vertical ellipsis appears with a dropdown menu containing the Edit, Details, Delete links. I utilized CSS to hide the ellipsis button until hovered over, and javascript for the dropdown funcationality. I then added CSS icons next to the Edit, Details, and Delete links.
- [INDEX PAGE](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/indexCrud.png)
![](https://github.com/esievaughn/TheaterMVC/blob/main/CSharp-MVC/indexpage.png)
