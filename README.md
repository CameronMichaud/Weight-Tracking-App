# CS-360-Mobile-Architecture-and-Programming
<div align="center">
  <img src="App Code Design/Updated UI/Data.jpg" width="32%"/>
  <img src="App Code Design/Updated UI/Login.jpg" width="32%"/>
  <img src="App Code Design/Updated UI/Goal.jpg" width="32%"/>
</div>
<div>
  <img src="App Code Design/Updated UI/AddWeight.jpg" width="33%"/>
  <img src="App Code Design/Updated UI/EditWeight.jpg" width="33%"/>
</div>

___

**Goals:**
The goals of this app were to develop a daily weight tracker that allowed a user to:
- Login to a database, display results related to the user
- Store daily weights in a database where a user could create, read, update and delete entries
- Display weights in a grid where a user can perform database actions on them
- Set a goal weight
- Have the app notify the user through SMS once they've reached their goal weight
___

**Screens:**
- Login screen
- Daily weight list screen
- Weight adding screen
- Weight editing screen
- Set goal weight screen
___
**UI**
- The UI for my screens were designed with the ergonomics and readability of the user in mind. Editing/Adding weights and setting a goal weight are all encapsulated in their own screens and alert dialogs to enhance readability of each screen and related functions are all placed close to one another with less often used buttons regulated to the corners of the screen where the user would have to expend the most amount of energy to interact with. For selecting a weight & date I chose to use widgits that could allow a user to not have to interact with their keyboard to limit the amoung of changes the user has to make to their interactions with the screen to achieve functionality.
___
**Developing**
- I approached developing this app by focusing down a single feature at a time and testing to make sure the feature worked completely before moving onto the next. I didn't utilize unit testing during this project and instead I made the extensive use of log statements to gain an understanding when errors occured that I could not find the origin of, in hindsight I see how utilizing debug would've suited a lot of these situations better. This process was much more helpful than I had given thought at the start of development and it is a skill I hope to improve on with future projects by developing with a testing-first mindset.
___
**Challenges**
- I encountered a number of challenges during development that I had never experienced in past courses which largely centered on calling between classes, running into some static/non-static errors, and a significant amount of difficulty implimenting the SQLite database with it's multiple tables and SMS message sending & obtaining necessary permissions from the user to ensure all features ran properly. All of these required me to go back and really understand what was causing me the issues I was having and resulted in me having a strong understanding of how classes can interact with one-another and how to initialize & act upon a SQLite database.
___
**What Was Done Well**
- An element that doesn't outwardly show the amount of understanding it took to create was a custom dialog box I made for the goal weight selector screen that had three number pickers inside of it that would remove the last goal weight, add the new one, and then update a custom data type that had a goalWeight field to finally write to the text value of the button that originally spawned the dialog box "Tap to set". All of the major components that I had issues with in this project and some significant lessons I've learned in past coding classes all culminated into a large function that called other private class methods and public methods from seperate files while also using a good amount of overloading and polymorphism to try and keep the code readable & efficient with it's resource allocations. There was definitaly sections that could be consdiered more complex but I found that function specifically to be a good test of the principles I know so far in software development.
