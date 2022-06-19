# What is PHP? :thinking: :question:
 
- PHP (Hypertext Preprocessor) is known as a general-purpose scripting language that can be used to develop dynamic and interactive websites.

### Some uses of PHP : 
   
  - PHP performs system functions, i.e. from files on a system it can create, open, read, write, and close them.

  - PHP can handle forms, i.e. gather data from files, save data to a file, through email you can send data, return data to the user.

  - You add, delete, modify elements within your database through PHP.

  - Access cookies variables and set cookies.

  - Using PHP, you can restrict users to access some pages of your website.

  - It can encrypt data.

### Syntax :

   ```
    <?php
      echo "Write Code Here.";
    ?>
 
   ```
### Echo :
  - Echo is used to output data to the screen.
  
  - The echo statement can be used with or without parentheses : echo or echo().

  - For Example : 
  
  ```

  echo ("Hello World <br>");
  echo "Hello world";
  ?>

  
  Output : 
  
  Hello World
  Hello world
  
  ```
  Here, both outputs are displayed regardless of the parantheses ().

# Virtual Host :

## What is Virtual Host? :question:

The term Virtual Host refers to the practice of running more than one web site on a single machine. Virtual hosts can be "IP-based", meaning that you have a different IP address for every web site, or "name-based", meaning that you have multiple names running on each IP address. The fact that they are running on the same physical server is not apparent to the end user.
  
 
## How do you setup virtual host? :thinking:

  - First download XAMPP by :arrowright: [clicking here](https://www.apachefriends.org/) :arrowleft: .

  - Install it in your C: directory.

  - Open XAMPP COntrol Pannel and turn on `Apache` and  `MySQL`.

  - Then move your folder `wt-lab-assignment` to `C:xampp\htdocs\`.

  - Now, open the file `httpd-vhosts.conf` from the path `C:\xampp\apache\conf\extra` in notepad(running as administrator) and add the following code.
 
    ```
   <VirtualHost *:80>
   DocumentRoot "C:\xampp\htdocs\wt-lab-assignment\Assignment7\"
   ServerName Hello.local
   </VirtualHost>

   <VirtualHost *:80>
   DocumentRoot "C:\xampp\htdocs\wt-lab-assignment\Assignment\Assignment7\"
   ServerName Second.local
   </VirtualHost>

    ```
  - Then to path `C:\Windows\System32\drivers\etc` and open the file `hosts.conf` in notepad(running as administrator) and add :
    
    ```
     127.0.0.1       Hello.local
     127.0.0.1       Second.local

    ```

  - Now, open your browser and search `localhost\path of your directory`. :white_check_mark:
  