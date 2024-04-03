## Task List

https://a3-sethfrank.onrender.com/

This application is to be used for creating a task list, specifically for classes that someone is taking. It includes fields for the user to input a task, the class associated with it, the due date and importance of it. Some challenges I faced in creating the application were getting the database setup, especially with making sure that tasks for each user were showing correctly and not showing other tasks. 
For authentication, I use a simple username and password system that is stored within a database. When loading the application, the user is prompted to enter in a username and password which will then be checked with the information in the server. If the username doesn’t exist, it will create a new user with the inputted username and password. If there is that username but wrong password, it will show login failed. And if both the username and password are correct, it will bring the user to their tasks. I choose this system as it was not too complicated for both myself and for the user who will be logging in as it is just a simple username and password.
I used Bootstrap for my CSS framework. I choose this since it is a widely used framework that many web applications use. It also had simple but modern looking styles that are great for any web applications. It also allowed for easy customization for choosing which elements to apply a style to as well as changing things like colors and such.

Middleware
-	Cookies: Used for creating keys for encryption
-	Sending unauthenticated users to login page
-	Middleware that sends an error if the collection doesn’t exist in the database

Logins
- Username: test    Password: test
- Username: test2   Password: test2


## Technical Achievements
- **Tech Achievement 1**: Hosting on alternative service: I decided to use Render as a hosting service. I’m using the free version and using web service hosting. Besides it taking me forever to figure out that I needed a web service and not a static site, it was very easy to set up. I just needed to add in my environment variables and the rest was all set up through my package.json file that was already there. Overall, Render is great with the auto-deployment when changes are pushed to main and works fairly well speed wise given the free version. Overall it seems better than Glitch given the auto-deployment and more functionality with changing settings and such. Although, you can’t edit things directly in Render unlike Glitch.
- **Tech Achievement 2**: I got a 100% in all of the Lighthouse scores for desktop.
- **Tech Achievement 3**: For one of my tech achievements, I decided to add the ability to add tasks to another person’s task list from your own. The thinking behind this was in case you are collaborating with someone and want to assign the task to them as well so they have it on their task list. The way it works is that when adding a new task, it allows the user to check off a username that they would want to assign the task too. They can check off multiple people or check off no one if it is just a task for themselves. It will then add a copy of that task to the other person. Therefore, you cannot edit or delete the task on the other person’s account but only add one onto it.

### Design/Evaluation Achievements
**Design Achievement 1**: Implement 12 Tips from W3.org
1.	Provide sufficient contrast between foreground and background: For the background, I have an off shade white with black text throughout. All the colors I used are not too bright and are more dull colors in order to make sure doesn’t blend in too much but also not too bright.
2.	Ensure that interactive elements are easy to identify: For all my buttons, they change a shade of color when they are hovered over. It also changes the cursor to identify that it is clickable. For the radios, it also changes slightly to show the user that they can click and the cursor changes. And then my field inputs change cursor and highlight in blue when clicked to show that the user can type something.
3.	Ensure that form elements include clearly associated labels: For my form inputs, all of them have labels to the left of the input as well as the text inputs having placeholders in the field indicating what to enter.
4.	Provide easily identifiable feedback: When the user forgets to input in one of the fields or inputs the data incorrectly, it will give feedback in the form of an alert to tell the user to input or change how they inputted the data.
5.	Create designs for different viewport sizes: When the width of the screen is smaller, it will put the labels for each input above the input field so that there is more room for the user to enter text. The table also sizes based on the width of the screen, making it adaptable for many screen sizes (although it does have a min width of around 600px).
6.	Provide clear instructions: When the user doesn’t input things in the input fields correctly, I give information instructions on how to fix including things like fill in all the fields or input the date in the specified format. This makes it clear that all the inputs need to be filled in for the user to be able to submit a task.
7.	Associate a label with every form control: Each of my inputs for both sign in and the submitting data has a label associated, making it easy to see when reading the code and for the user as well.
8.	Identify page language and language changes: I indicated the language as English on every page.
9.	Help users avoid and correct mistakes: I provide clear instructions if the user inputs data correctly so that they know what they need to change and where to change it.
10.	Reflect the reading order in the code order: All the code in the HTML displays in the way that it is displayed in the app with everything that is visually on top, also on top in HTML.
11.	Write code that adapts to the user’s technology: The code specifically for the table is meant to adapt to the user’s screens width as well as the input fields adapting to the width and changing the position of the labels if it gets below a certain width.
12.	Don’t use color alone to convey information: Everywhere that I use color, it is in addition to text that is used with it. This allows things to have emphasis with the color but still makes it clear with what it is for.

**Design Achievement 2**: Following CRAP Principles
- Contrast: For the use of contrast, I used colors to help with emphasis of elements on the page. With the table results, the table was a different color than the rest of the page to put emphasis on it and lead the user to looking at that. This was the element that had the most emphasis on the page with it being large and using the color to emphasize it. I also used font size and utilization of bolding to make the titles like “Add Tasks” and “View Tasks” to pop, allowing the user to easily tell which section is which. I also emphasized the Submit and Logout buttons by making them a bolder color to signal to the user that these are important. However, the edit and delete buttons are not as emphasized since they are gray. This is because there are a lot of these buttons and not as important as the others. 
- Repetition: One way I use repetition is with the use of bolding for all the titles and subtitles in the page. This makes it easier for the user to navigate through the page. I also use repetition for all the input fields for submitting data by making them all the same size and looking consistent with text. This makes it easier for the user to navigate through each field and input the correct values. I also used repetition with the table. It repeats the alternation of the colors as well as keeping all the text and spacing consistent as well as the same buttons for each row. Again, this makes it a lot easier to navigate and find the right information that the user is looking for.
- Alignment: When looking at my table, I keep the alignment consistent throughout. First, all the elements are aligned to the left, creating consistency and making it easier for the user to read since the elements are different sizes of text (as compared to doing center align which wouldn’t be as visually appealing). When looking at the adding tasks, these are also aligned to the left with each input field being aligned together both horizontally and vertically. The radios for the importance input are also aligned with the other input fields to create this consistency. Also when looking at my login page, everything here has a center alignment since the elements are smaller and makes more sense to fill up the page in the middle instead of on a side.
- Proximity: One way I used proximity is in my table. First, I put the task and class elements next to each other since they are both text-based answers and relate to each other. Then I also put importance and priority next to each other since they are related, allowing the user to see both of them together. I also have the edit and delete button together since they are both buttons that will lead to modification of the task. Also with the Log Out button, I have the username of the person right next to so that when you are logging out, you know which account you are signed into before you make the decision to logout. Also more obviously, all the things for adding a task are in near proximity to each other as well as all the things for displaying results with the table instead of being spread out all over the page.