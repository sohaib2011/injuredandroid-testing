# Flag 2 - FlagTwoActivity

<img src="https://github.com/user-attachments/assets/88182862-75dd-4adf-befd-7450154243ca" width="150">

**Hint #1** - Key words Activity and Exported

**Hint #2** - Exported activities can be accessed with adb


The provided hints gave us a lead regardin the flag, indicating that we should delve deeper into the AndroidManifest.xml sourcecode.
AndroidManifest is the core config file for the app, and among the key components is **Activity**.

1. 237 lines of code so we can narrow down our search to 'exported="true" to find what we want to look for. As a result we found potential matches; one being b3nac.injuredandroid.b25lActivity, and another b3nac.injuredandroid.QXV0aA
<img src="https://github.com/user-attachments/assets/1a29c297-17a2-4c7d-942d-2a80a32d3cb0" width="500">


<img src="https://github.com/user-attachments/assets/dc499570-b4b9-48a5-803e-6cbe59565091" width=380>


2. The idea behind activities marked as exported=true, is that we can access certain UI elements directly from our phone without having to navigate through the app itself.

 
 To exploit this, we can run the following command:
 <img src="https://github.com/user-attachments/assets/7f24ecbb-496b-408f-9cb7-61aab73988ba" width="100">

part between / is the package name, and the part after is the activity being launched.

3. By launching the exported activity directly, we managed to bypass the FlagTwoactivity screen and discovered a hidden flag
<img src="https://github.com/user-attachments/assets/14a0aedd-502a-4d53-9abe-46569ac931cf" width="200">

   
