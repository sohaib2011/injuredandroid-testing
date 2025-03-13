# Flag 3 - Resources 

bilde

#### **Hint #1**  
R stands for **resources**  

#### **Hint #2**  
Check **.xml files**

---

Tried searching for any clues directly in AndroidManifest.xml with no luck. The second option is to read directly into the sourcecode for the UI for FlagThree

<img src="https://github.com/user-attachments/assets/c6be8d77-4708-4a45-86e7-7000d4cde3a3" width="600">

1. The code above tells us that the function allows user to input a string, and if it matches a string in 'R.string', it will output something interestering. Lets use 'cmVzb3VyY2VzX3lv' to inspect further
2. By inspecting into the /res/values/string.xml path we managed to find a hidden string for our flag. 
   
   <img src="https://github.com/user-attachments/assets/754469be-7b37-4ef4-87b7-c97649b3325c" width=400>

3. Well that was easy
   
   <img src="https://github.com/user-attachments/assets/af04dcd9-94aa-4783-8bf2-1194c8789601" width=200>
