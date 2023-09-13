# WESTERN GOVERNOR UNIVERSITY
## D287 – JAVA FRAMEWORKS

C. Customize the HTML user interface for your customer’s application. The user interface should include the shop name, the product names, and the names of the parts.

File: mainscreen.HTML
Line #: changes

14: Changed title to My Drum Set Store

19:Changed text in h1 tags to Tempo Treasures

40-64: Added list of Parts (name, price, inventory)

101-125: Added list of products (name, price, inventory)


D.  Add an “About” page to the application to describe your chosen customer’s company to web viewers and include navigation to and from the “About” page and the main screen.

File: about.HTML
Line #: changes

 1-38: Added a new html file under templates name about.HTML, I set up a basic page with a title and paragraphs using thymeleaf
 34: I added a button that leads back to the mainscreen labeled Back to Home

 File: AboutController.JAVA
1-13: I added a controller class called AboutController under controllers,
6: i added the annotation to mark it as  controller @controller
9: mapped the about.html by using @getmapping(/about)
20-13: made a method that returns the about page.






E.  Add a sample inventory appropriate for your chosen store to the application. You should have five parts and five products in your sample inventory and should not overwrite existing data in the database.

File: BootStrapData.JAVA
Line #: changes

59: Added an If statement that checks the count of productRepository and partRepository to makes sure they are zero
61 - 105: added the 5 new objects of parts
107: Fetching all OutsourcedPart instances from the outsourcedPartRepository.
108 -116: Iterating through each part and checking if its name is matches the case then sets thePart# equal to Part
118 - 122: makes a new Product from the product class
124 -133: saving 5 outsourceParts and Products to their respective repositories.





F.  Add a “Buy Now” button to your product list. Your “Buy Now” button must meet each of the following parameters:



G. Modify the parts to track maximum and minimum inventory by doing the following:




H. Add validation for between or at the maximum and minimum fields. The validation must include the following:



I.  Add at least two unit tests for the maximum and minimum fields to the PartTest class in the test package.


J.  Remove the class files for any unused validators in order to clean your code.
