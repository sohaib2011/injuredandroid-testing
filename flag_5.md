# Flag 5 - Exported Broadcast Receiver

<img src="https://github.com/user-attachments/assets/4246c0ce-9a76-4973-a14a-8f9edb7702e3" width="150">




As seen in the image above, the activity revealed only a white screen with a small popup. Since i was used to getting hints and didnt find this sufficient enough, i spammed the activity until i accidently revealed the flag haha

![image](https://github.com/user-attachments/assets/62102d6a-dd32-49a3-ba5e-3118669ee60b)


1. Revealing the flag doesnt suffice me, so i want to understand more in depth to what is happening behind the scenes. By inspecting the source code for FlagFiveReceiver, we can see some key points:
   * f1454a increased everytime onReceive ran, which we can see it increased from 0 to 3. After that it reset to 0 and continued its loop
   * The base64 encoding seems to be our flag. I tried directly decoding it through cyberchef but it seems like it is scrambled with other mechanisms. Seems like my "accident" wasnt an accident.
   
   <img src=https://github.com/user-attachments/assets/afe49787-17b3-4d4a-9ea5-4b0435485c91 width=450>



