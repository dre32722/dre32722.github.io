
# Explore the APIs using an Online Python Service

One of the nice thing about modern APIs, is that we can choose our favourite programming language to access them. In this section of the handson lab you will 

## Get the code snippet from Postman
If you have been following through the handson labs you will already have a Postman collection with your Get and Post operations to access the APIs already saved. 
Perform the Get operation to prove it is still available and responsive.
<br>
<img src="./img/postman1.PNG"/>
<br>
Click on the Code link (it is located just under the Save button). 
In the top left of the dialog window you can select the grey button (top left) and choose the programming language that suits your needs. For the purpose of our labs, choose, Python - http.client(Python 3)
<br>
<img src="./img/postman2.PNG"/>
<br>
Copy the code snippet to the clipboard buffer.
<br>
<img src="./img/postman1a.PNG"/>
<br>
## Paste and run the Get Physicians code snippet into an online Python service
<br>
Once you copied the Python snippet then you can run it wherever you want. 
There are several options that you may consider;
1. Run it in your own existing Python environment,
2. Install python locally and run it there 
3. Download a Python docker image from Docker hub
4. For simple scenarios such as what we want to cover, you could simply use a browser-based IDE offering such as what * [TutorialPoints.com](http://tutorialPoints.com) offer, as per the steps below.
<br>
Point your browser to [TutorialsPoint Python](https://www.tutorialspoint.com/execute_python3_online.php)
<br>
<img src="./img/pythoneditor1.PNG" />
<br>
You should see a Hello World example waiting for you. 
Press the Execute Button to see Hello World returned into the console window below the code editor.
Notice in the console window that the command being executed is as follows;
*python main.py*
<br>
<img src="./img/pythoneditor2.PNG" />
<br>
Next create a new file within the pre-established project.
Click the '+' symbol in the Project pane (left of the code snippet) to create a new file.
Right Click on the new file to rename it - *GetPysicians.py*
Now clickon the tab for the GetPhsicians.py file and paste your clipboard contents that you copied from Postman into the code editor. 
In the console window type the following;
*python GetPhysicians.py*
All being well in the universe you should see the Physicians you added earlier returned.
<br>
## Repeat for Post Physicians 
<br>
In Postman execute a request to Post a new Physician.
Repeat the step to copy the code snippet.
Create a new file called *PostPhysicians.py* in the project on tutorialspoint website.
Execute the following command
*python PostPhysicians.py*
Observe the response
Now in the console window type the following;
*python GetPhysicians.py*
You should see the Physicians you added earlier plus the one you just added.
<br>
* No warranty expressed or implied.  Software is as is.
* [MIT License](http://www.opensource.org/licenses/mit-license.html)
<br>
<hr />
<center>
<a href="../../handsonlabs" class="btn" >Back to Hands On Lab Menu</a>
<center/>
<hr />

