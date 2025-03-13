# Flag 2 - Exported Activity

<img src="https://github.com/user-attachments/assets/88182862-75dd-4adf-befd-7450154243ca" width="150">

#### **Hint #1**  
Key words: **Activity** and **Exported**  

#### **Hint #2**  
Exported activities can be accessed with **ADB**

---

The provided hints gave us a lead regarding the flag, indicating that we should delve deeper into the **AndroidManifest.xml** source code.  

AndroidManifest is the core config file for the app, and among the key components is **Activity**.

---

1. With **237 lines of code**, we can narrow down our search to `exported="true"` to find relevant activities.  
As a result, we found two potential matches:

- **b3nac.injuredandroid.b25lActivity**  
- **b3nac.injuredandroid.QXV0aA**

  
<img src="https://github.com/user-attachments/assets/1a29c297-17a2-4c7d-942d-2a80a32d3cb0" width="500">


<img src="https://github.com/user-attachments/assets/dc499570-b4b9-48a5-803e-6cbe59565091" width=380>


2. The idea behind activities marked as exported=true, is that we can access certain UI elements directly from our phone without having to navigate through the app itself.

 
 To exploit this, we can run the following command:
 <img src="https://github.com/user-attachments/assets/7f24ecbb-496b-408f-9cb7-61aab73988ba" width=1600>

The part between `/` is the **package name**, and the part after is the **activity** being launched.  


3. By launching the exported activity directly, we managed to bypass the FlagTwoactivity screen and discovered a hidden flag
<img src="https://github.com/user-attachments/assets/14a0aedd-502a-4d53-9abe-46569ac931cf" width="200">

   
