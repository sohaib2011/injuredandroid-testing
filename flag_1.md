# Flag 1 - LoginActivity

1. The hints "the flag is under your nose and GUI" suggests that we should inspect beyond the application and into the source code. A good approach for this to analyze the APK file by using JADX-GUI

<img src="https://github.com/user-attachments/assets/4dbed37a-35ed-4169-8586-34db56d49bb2" width="250">



3. After opening .APK in JADX, we can navigate to the **b3nac.injuredandroid** package and locate the source code for **FlagOneLoginActivity**, as shown below:
 
   <img src="https://github.com/user-attachments/assets/cea7eedf-fae8-4b54-99b3-05846bb003ba" width="650">  

4. By exploring this activity, we find a function responsible for handling user input.
   
   <img src="https://github.com/user-attachments/assets/ed7eae67-b9f2-4d10-a425-93d2e033e2d4" width="650">  

   This becomes evident that the function compares the entered value against a predefined string 'F1ag_0n3', which will reveal the flag. Lets test it out on the actual application...

5. We have a match! Looks like the string'Flag_0n3' is the correct flag
![image](https://github.com/user-attachments/assets/679105bf-a5cd-4de0-81ce-f04740939616)

