# wicsme2020-writeups (0xL4ugh)
<h1 align="center">Digital-Forensic-Challenges </h1>   
 
 
*****************************************************************************************************************************************************************
<h2 align ="center ">Fe01</h2>
</br>
It was an easy one there was a .rtf file when i opened it using ("libre office Writer") i found: </br></br>

![1](https://user-images.githubusercontent.com/33530187/99195681-2c11ce80-2755-11eb-9103-01f23bf3878b.png)

</br>

by clicking (Ctr+A) I selected all the right clicked to choose paragraph - Text Body </br>
</br>
![2](https://user-images.githubusercontent.com/33530187/99195858-6039bf00-2756-11eb-9cad-21085cd6eca9.png)

the flag appered</br>
![flag](https://user-images.githubusercontent.com/33530187/99195866-6e87db00-2756-11eb-8217-1e0b8d33ae59.png)

the flag was :<b>n𝑖𝐶𝑒𝐴𝑛𝐷𝐸𝑎𝑠𝑦10018</b>
*****************************************************************************************************************************************************************
</br>
<h2 align="center">Fe02</h2>
</br>
it was a PDF File with a black mark that hide some parts of the text, I Opend it using ("Atril Document Viewer") </br>
And that what appered: </br>

![1](https://user-images.githubusercontent.com/33530187/99196046-d854b480-2757-11eb-9ae6-3b515dd35fd8.png)
</br>
i was going to reverse the pdf but i noticed Some thing when i highlight a text it appers </br>

![2](https://user-images.githubusercontent.com/33530187/99196086-18b43280-2758-11eb-9e4b-730207412d80.png)
</br> 
so I easily selected the hole file and found the flag:</br>
![flag](https://user-images.githubusercontent.com/33530187/99196138-616beb80-2758-11eb-8283-08642fd67fbf.png)
</br>And the flag was :<b> n1CeReDaCTION-sureLYNot911081</b>

*****************************************************************************************************************************************************************
</br>
<h2 align="center">Fe03</h2>
when i unzipped the challenge there was a flag.zip password protected</br>
so I knew it's a simple password cracking Challenge </br>
using zip2john I got the hash  </br>
![1](https://user-images.githubusercontent.com/33530187/99196407-35ea0080-275a-11eb-90b9-10b8318d5f7c.png)
</br>
Then by using Rockyou.txt to brute force The password it succeeded</br> 
![johend](https://user-images.githubusercontent.com/33530187/99196524-d9d3ac00-275a-11eb-8496-6344bc0cc74b.png)
</br>

and the password was :
<b>q1w2e3r4t5y6</b>
by using this passsowrd i was able to extract the text file :</br>
![flag](https://user-images.githubusercontent.com/33530187/99196624-988fcc00-275b-11eb-9d4b-25effcf52bb9.png)
</br>

the flag was  :<b> CraCKInGJ0b-67189 </br>
*****************************************************************************************************************************************************************
</br>
<h2 align="center">Fe04</h2>

it was an .log file So i tried the first thing I could think of </br>

using the command strings with grep flag </br>

so I did that </br>

```bash
strings access.log |grep flag
```
</br>
and that was it the flag appeared  </br>

![flag](https://user-images.githubusercontent.com/33530187/99196830-c1fd2780-275c-11eb-8e9f-bcc4aaa416bf.png)
</br>
the Flag was: <b> nicESearChIng01812</b> 
*****************************************************************************************************************************************************************
</br>
<h2 align="center">FM01</h2>
It was a weird file i used file to idintfy it but it showed Data file </br>

![1](https://user-images.githubusercontent.com/33530187/99196983-7a2ad000-275d-11eb-80bf-e3c125484c95.png)
</br>
so i opend it on hex editor to see the header </br>

![2](https://user-images.githubusercontent.com/33530187/99197077-2c629780-275e-11eb-9e39-5e9bb123adb8.png)

</br>
the Hex was similar to a binary file but the header was wrong</br>
So i fixed it by adding the right header</br>

![the fixed header](https://user-images.githubusercontent.com/33530187/99197901-51a5d480-2763-11eb-997e-f2cfac8f87df.png)
</br>
and by using 
<b>
 
```bash
chmod +x file| ./file
```

</b>

![flag](https://user-images.githubusercontent.com/33530187/99197986-bbbe7980-2763-11eb-858f-6b6b2d070dee.png)

</br>


*****************************************************************************************************************************************************************
</br>
<h3>
and sadly we couldn't solve The last 2 challenges (FM02 , FH01)
</h3>
