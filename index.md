# Vilaysith Phongsavath - SNHU Capstone ePortfolio
## CS-499
------------------------------------------------------------

### This portfolio contains three programming projects, a video, and a self assessment
### Final - Self Assessment
### Milestone 1 - Code Review and Plans (Video)
### Milestone 2 - Software Design and Engineering (pet.java,jframe)
### Milestone 3 - Data Structures and Algorithms (petsView.java,jframe,mysql) 
### Milestone 4 - Databases (registration.java,jframe,jdbc,mysql)

-------------------------------------------------------------

## Self - Assessment:

### Overview:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;More than an achievement I have accomplished through the course and that shows up in multiple skills I gained and used them to enhance the code starting from the software design category where I focused on delivering quality work and sharing a clear code to build up a collaborative environment, moving to the data structure section where I used some new algorithms and applied new practices while managing the trade-offs involved earlier in the software design. 
Finally, in the databases category where I used a simple artifact and connected it to the existing code, in addition, I surfed the internet to get some workarounds to be able to use the available tool NetBeans and I was able to accomplish the task successfully.
I noticed that I have a better security mindset in all the project categories, especially while creating the access to the database administrator, however, I feel that this part should be improved in the future as I need to always keep in mind that passwords must be complex to avoid easy cracking, so the combination of uppercase, lowercase letters, numbers, and special characters is mandatory all-time in the code; either if I am the user who is creating the credentials or I am the developer who is developing the code. 
So, I will consider this part in the future and I will make sure to add a clear pop-up in such a case to educate the users on how to create complex passwords. This point shows up that I become more proactive and my productivity is improved over the course.

#### Team Environments:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;When it comes to collaborating in a team environment,Learning how to use Git helped me to better understand its various features. I think that it is the main source of collaboration and team environments. Having this knowledge is very important for any team member.

#### Communicating to Stakeholders:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I believe that my projects directly communicate with stakeholders. The program I develop allows the stake holders to be able to easily add or delete their pet also veiw all of the pets in the database.

## Milestone 1 - Code Review video
link to the code review https://www.youtube.com/watch?v=ko3zrZhegww&t=5s

## Milestone 2 - Software Design and Engineering
### Converting original command line txt java code into a more user friendly graphic user inteface with added security features in a form of a username and password

#### Artifact Description:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;My artifact for milestone two is based off of a project from my IT-145 course.I used the pets’ shop code I developed earlier in IT-145 (Foundation in Application Development). This artifact was created around October 2019, I have learned a lot of concepts since then so I used these qualities in enhancing the software design and code structure and link it with another search engine structure code I created later in CS-260 (Data Structures and Algorithms: Analysis and Design) in early 2021. 
Java Swing JFrame class is the main artifact I used in this part to enhance the graphical user interface as it is typically the foundation for creating graphical Java applications. So, I imported javax.swing package. Also, I used the JDialog package to control the top-level window while inserting the Pets’ data, it inherits the Dialog class and it is a part Java swing package, I used this class as it can be customized based on the business need. Basically, the JDialog constructor is used to initiate a modeless dialog without a specified Frame owner and without a title.

### Artifact Enhancement Process:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Quality work starts by keeping every single detail in the project documented, I added more comments in the code to clarify the purpose of adding each portion of the code, I ensured to declare all the variables and that helped me to avoid Undefined Errors. So, I see that I succeeded in keeping the software design clear and simple which is one of the main course outcomes.

### Artifact inclusion:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;By using javax.swing package, I enhanced the code design so both the administrators and users can navigate between tabs easily and the new design allows the users to enter the pets’ data easily which is a great skill I learned over the course; when it comes to delivering a professional design, we should deliver a quality work that gives the end-users oral, written, and visual communications and make them feel that the application design is friendly.

## Milestone 3 and 4 - Algorithms and Data Structures and Databases

#### Artifact Description:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I used the Binary Search Algorithm to perform the search on the pets’ dataset. It counts on continuously dividing the whole portion of the list into chunks that could contain the required item until it narrows down the results to one possible item by using the time complexity O(log2N). I imported the dataset java.sql, then, started applying this methodology to the code, after that, when you search for the name of a pit in a sorted list of pets, the algorithm performs the binary search to return the best match based on a string-matching on the stemmed keywords.

### Artifact Enhancement Process:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Currently, I know more about data structure techniques and how are they breaking data down into terms to easily store them in the database and call them quickly when running the queries which is called the indexing process, basically, this helps in minimizing the number of disk accesses while processing queries, in addition, in large databases, we do not need to hammer databases each time we call an item. The search terms are generated using an analyzer that stems each word to its root form, this process helps the system in suggesting results according to the stemmed keywords. 
This artifact helped me use one of the skills I gained over the course and that shows up in using new packages like java.sql and ensured to declare all the variables in the program, also, I loaded MySQL driver successfully to the registration code and developed a connection between the local JDBC MySQL driver and the portal that is developed by java initially 

### Artifact inclusion:
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;I created a portal to be able to search for pets and filter them easily, I used some other known algorithms such as BFS (Breadth-First Search) or DFS (Distributed File System) for data indexing and getting the results easier and faster from the database, this practice evolved my experience in both linear and binary searches and helped me practically in enhancing the current software code and creating the portal view in a practical way.
I added a new portal view in the code structure so when users click on the View Pets button, it shows up another window and lets the users be able to start searching in DB.I imported java.sql to get all classes from the package java.sql at once, then, completed the connection setup by declaring the DB location and credentials to allows the code issues SQL queries to the database, I noticed that the password is not complex at all which is something I will keep in mind in a production environment for security purposes as the security mindset is one of the helpful concepts I learned over the course. Other than this, I added an insert method to insert the pets’ values into DB and to show up the message Saved Successfully once the record is inserted properly. In addition, I added a quick catch that an error has occurred when you cannot find what you are looking for, this is one of the most interesting concepts I learned in this course, I should give the user a clear error message to help identify and troubleshoot the issues easier.

###  Link to Milestone two: Original pet.java and enhancement pet.java code
https://github.com/phongsavathv/phongsavathv/commit/b80897d7a63b87423d692d8d697cf720e22bafe9

### Link to Milestone three:  Algorithms and Data Structures enhancement code
https://github.com/phongsavathv/phongsavathv/commit/f5c1c060395c25f16f030d29f774cbfbd3895c98

### Link to Milestone four: Database enhancement code
https://github.com/phongsavathv/phongsavathv/commit/7356341f223e8a27125ed3f49fb2b3153dd9bfa7



