## Part 1
Code for `ChatServer`<br>
<img src = "chatserver.png" width = 400 height = 450><br><br>

Output 1<br>
<img src = "Main_page.png" width = 400 height = 100><br><br>

Output 2<br>
<img src = "Samson.png" width = 400 height = 100><br><br>
**Which methods in your code are called?**<br>
The handleRequest function is called everytime the page is refreshed<br>
**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**<br>
For my function, the argument and field valeus are assigned to the following:<br>
Revelant argument: `URL url` = http://localhost:4000/add-message?s=Hello&user=Samson<br>
Revelant fields of the class before calling: `output = ""`<br>
Revelant fields of the class after calling: `output = "Samson: Hello\n"`<br>
`String[] parameter = ["s", "Hello&user", "Samson"]`<br>
`String cateS = "s"`<br>
`String middlePString = "Hello&user"`<br>
`String userInput = "Samson"`<br>
`String strInput = "Hello"`<br>
`String cateUser = "user"`<br>
**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why**<br>

Output 3<br>
<img src = "Alex.png" width = 400 height = 100><br><br>
**Which methods in your code are called?**<br>
The handleRequest function is called everytime the page is refreshed<br>
**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**<br>
**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why**<br>
