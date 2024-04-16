## Part 1
Code for `ChatServer`<br>
<img src = "chatserver.png" width = 400 height = 450><br><br>

Output 1<br>
<img src = "Main_page.png" width = 400 height = 100><br><br>

Output 2<br>
<img src = "Samson.png" width = 400 height = 100><br><br>
**Which methods in your code are called?**<br>
The handleRequest function is called everytime the page is refreshed<br><br>
**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**<br>
For my function, the argument and field valeus are assigned to the following:<br>
Revelant argument: `URL url` = http://localhost:4000/add-message?s=Hello&user=Samson<br>
Revelant fields of the class before calling: `output = ""`<br>
Revelant fields of the class after calling: `output = "Samson: Hello\n"`<br>
Revelant fields of the method:<br>
`String[] parameter = ["s", "Hello&user", "Samson"]`<br>
`String cateS = "s"`<br>
`String middlePString = "Hello&user"`<br>
`String userInput = "Samson"`<br>
`String strInput = "Hello"`<br>
`String cateUser = "user"`<br><br>
**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why**<br>
Revelant fields of the class before calling: `output = ""`<br>
Revelant fields of the class after calling: `output = "Samson: Hello\n"`<br><br
                                                                              >
Output 3<br>
<img src = "Alex.png" width = 400 height = 100><br><br>
**Which methods in your code are called?**<br>
The handleRequest function is called everytime the page is refreshed<br><br>
**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**<br>
For my function, the argument and field valeus are assigned to the following:<br>
Revelant argument: `URL url` = http://localhost:4000/add-message?s=BOOM&user=Alex<br>
Revelant fields of the class before calling: `output = "Samson: Hello\n`<br>
Revelant fields of the class after calling: `output = "Samson: Hello\n"Alex: BOOM`<br>
Revelant fields of the method:<br>
`String[] parameter = ["s", "BOOM&user", "Alex"]`<br>
`String cateS = "s"`<br>
`String middlePString = "BOOM&user"`<br>
`String userInput = "Alex"`<br>
`String strInput = "BOOM"`<br>
`String cateUser = "user"`<br><br>
**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why**<br>
Revelant fields of the class before calling: `output = "Samson: Hello\n`<br>
Revelant fields of the class after calling: `output = "Samson: Hello\n"Alex: BOOM`<br><br>

## Part 2
On the command line of your computer, run ls with the absolute path to the private key for your SSH key for logging into ieng6.<br>
<img src = "private.png"><br><br>

On the command line of the ieng6 machine, run ls with the absolute path to the public key for your SSH key for logging into ieng6 (this is the one you copied to your account on ieng6 using ssh-copy-id, so it should be a path on ieng6's file system).<br>
<img src = "public.png"><br><br>

A terminal interaction where you log into your ieng6 account without being asked for a password.<br>
<img src = "no_password.png"><br><br>

## Part 3
I learned how to create public and private key that uses RSA encryption with `ssh key-gen` command.<br>
Another thing I learned is the `scp [file] [remote server directory]` command to make a copy of the local file in the remote server<br>
It's also interesting to create a web server myself and write functions that perform different actions based on the url passed in.<br>
For rest of the thing such as linux commandline and remote server, I have previous knowledge already. 
