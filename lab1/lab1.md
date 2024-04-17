## `ls`
- Command Line with No Argument<br>
<img src="ls.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1`<br>
**Why the output**: It simply displays the content inside `lecture1` directory<br>
**Is it an error?**: The output is not an error because `Hello.class`, `Hello.java`, `README`, and `messages` all fall under the `lecture1` directory.


- Command with a path to a directory as an argument<br>
<img src="ls_directory.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1`<br>
**Why the output**: The command will list the contents of the directory we passed in. We can think this functions as a "preview" of a directory, and the user will be in the same directory after executing the command.
**Is it an error?**: The output is not an error because `Hello.class`, `Hello.java`, `README`, and `messages` all fall under the `lecture1` directory.


- Command with a path to a file as an argument<br>
<img src="ls_file.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1`<br>
**Why the output**: `ls` shows the content of a directory, but the argument here is the path to a filename.<br>
**Is it an error?**: The output is not an error because when you try to `ls [filename]`, it will just repeat the name of the file or the abosulate path the user typed in that is after `ls`


  
## `cd`
- Command Line with No Argument<br>
<img src="cd_noArg.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `~/`<br>
**Why the output**: When no argument is given, the user will return to the home directory<br>
**Is it an error?**: The output is not an error because `cd ~` is the command executed when no argument is given.

  
- Command with a path to a directory as an argument<br>
<img src="cd_directory.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1/messages`<br>
**Why the output**: It goes in to the message directory that is inside the `lecture1` folder<br>
**Is it an error?**: The output is not an error.

  
- Command with a path to a file as an argument<br>
<img src="cd_filename.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1`<br>
**Why the output**: You can only `cd` into a directory but not a file<br>
**Is it an error?**: The ouptu is an error. The picture above shows that `cd` only suports a directory name as a argument.

  
## `cat`
- Command Line with No Argument<br>
<img src="cat_noArg.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: N/A because it's in the mode of reading data from standard input adn write them to standard ouput<br>
**Why the output**: It basically does nothing because it just repeat what's the user typed in. The `cat` command will end when user hit control+D to indicate the end of the file<br>
**Is it an error?**: The output is not an error.

  
- Command with a path to a directory as an argument<br>
<img src="cat_directory.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: N/A cause error<br>
**Why the output**: `cat` cannot show the content of a directory, only `ls` can.<br>
**Is it an error?**: The output is an error because `cat` only reads the content of the file and does not accept a directory path as the argument.

  
- Command with a path to a file as an argument<br>
<img src="cat_filename.png"><br>
**Absolute path before**: `/Users/wanfranek/lecture1`<br>
**Absolute path after**: `/Users/wanfranek/lecture1/README`<br>
**Why the output**: It find the README file under the `lecture1` directory and reads its content.<br>
**Is it an error?**: The output is not an error.

  
