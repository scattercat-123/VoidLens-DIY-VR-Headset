# VoidLens the DIY VR Headset that is compatible with SteamVR 👓

## Day 1: WHy i wanted to build the headset and research
My friend Lucas11 in the hackclub slack was trying to organize a ysws called beatsaber. Its about the beatsaber game, i rsvped but i needed a vr goggle for playing it and doing the ysws. So i told lucas that i will make a diy vr headset so i can play many games and also beatsaber! I mostly like shooting games btw.
And at the end i have a fuly finished Headset!!!! 😄

Today was researchh day. i have built and fpv goggle b4 but i havent built a vr headset. firstly i found an open source vr headset thing calle relativity. it had some limitations, but i learnt many things from the repo! such as which display to choose, how to mount it, which lens to attach, can i make it steamvr comatible etc etc.
I researched a lot and finally i decided i will use the [Dual LS029B3SX02 Displays](https://www.alibaba.com/product-detail/LS029B3SX02-vr-head-mounted1440x1440-2K-120Hz_1600064437271.html?chatToken=TDFKeWNGRlpkWFZTWmtkNFRYRnZjVWxhVTBsU2RVcHNkRVpKVTJsMlRteERiM0ZyWlhrM2VHMXhZeTkwTVVSb2RIQnFRMGxKTmtONE9GSllWWFFyVG5WeFFscFVhSEY1YnpVd05tbGxVWFpCYVRWUFdISjZNRXQ0TkdkdlZIRlhXV295T0VKVVVXSTVVRzlXSzBwMFNXOW1NRUkyY25oTVIwZFdSVUUxT1RoUVowZzJSR0l3Y0ZoS016SlZaSHBOYXpoNU1XSXhWRE5LTVdsdlNsWmlWV1YxTnpjck9HWnVUMEZaUFE9PSZ2ZXJzaW9uPTIuMC4w&encryptTargetLoginId=8pctgRBMALOJDWt9qv%2B9TTfMDQuOgz5s6wdkfYSa%2Bs4%3D) . 

<img width="281" height="280" alt="image" src="https://github.com/user-attachments/assets/5d100a2b-a470-4a7b-8db1-b368e1343b60" />


This is a good display since it has 1 for each eye and its 120hz 2k resolution.
I also found another open source headset called HadesVR which uses a ping pong ball so that cameras can track the headset! This system was implemented by me later on..

## Day 2: Lens holder build
Im going kinda slow but today i just finished a rough lens holder

<img width="789" height="629" alt="image" src="https://github.com/user-attachments/assets/5a58f8bf-049f-4207-9d95-43852e3000be" />

Which i will modify a lot later on.

## Day 3: PCB Starting build
IDk why is tarted cad and switched to pcb, first i needed an hid compatible mcu which a sparfun pro micro will suit the best. i also added an led for the tracknig and a MPU9250 9dof motion sensor. my pcb schematic is below:
<img width="719" height="358" alt="image" src="https://github.com/user-attachments/assets/18bca190-be53-410e-ae5b-ad21c4e3de42" />

I also started assigning footprints and routing but i did it only halfway..

## Day 4: PCB and cad
I finished routing and you can see the final ugly result here:

<img width="720" height="439" alt="image" src="https://github.com/user-attachments/assets/385fa570-7c4a-4d60-ae76-492793b6e0a1" />

Here is a 3d view:

<img width="878" height="719" alt="image" src="https://github.com/user-attachments/assets/178d1806-4e6e-477b-b904-bf78c34a6a76" />

I also started modeling the Body!

## Day 5-7 : Cad modeling grind

I started modeling cad, i faced many problems like the lens holder i made earlier was nnot adjusted according to my IPD and once i measure my ipd through an app, it was about 60mm. So i fixed that and later when i tries to fit the lens holder to the body, the lensholder was too big, i had to cut it out which reusluted on it not being centered.
I also added little mounting grooves with brass insert for holding the lens holder:

<img width="491" height="470" alt="image" src="https://github.com/user-attachments/assets/0e33fb0b-9b0e-4446-b628-725f25765853" />

After this i found a mount for my display in relativity but it dint fit my ipd and all, i used the same display dimensions while adjusting for it to fit my body and my ipd, here is my final result,

<img width="709" height="752" alt="image" src="https://github.com/user-attachments/assets/2110cc41-3263-4b8b-bfee-4f023b813d40" />

I also had to keep in mind the distane between the lens and eyes and also the distance between the display and lesn should be calculated according to the type of lens im using..

Once that was done i did lotss of final adjustments to make sure they fit.

## Day 8: Modeled the Pcb holder, aesthetics

Today i modeled the pcb holder which you can see below

<img width="301" height="582" alt="image" src="https://github.com/user-attachments/assets/aa8ed3fc-82cc-4d98-b574-1ae53dee8731" />

IM done with the outer plate too! it has some branding btw:

<img width="516" height="584" alt="image" src="https://github.com/user-attachments/assets/d279cbcb-26eb-4bea-9b54-ea991fb8c632" />

The outer plate also has screw holes!

## Day 9: Final changes, adding ping pong ball.

I added the ping pong ball, did few fitting checks, and finalized everything.

Final result:

<img width="663" height="550" alt="image" src="https://github.com/user-attachments/assets/eaff9845-5713-43d4-a50f-41c25a39a680" />

# If you made it till here i cant believe that you understoof wahtever i wrote, cause idc about typos and my grammar is bad sry!
Thanks! Any suggestions? just create a issue/PR


# Thanks Alex and others for the questions!
## How will you connect the displays to the LS029B3SX02 dual displays?
 - Basically the driver has a DP(display port) . If you see my BOM i have an active dp to hdmi adapter. thats how i will mirror my steam vr to the display!

## The mpu is trashy..
 - I dont think so.. Even if its trashy many mpus have the same pinout so i guess i can just change

## Whhats the ping pong ball for.
 - Explained in the journal. please check out hades vr guide too if your unsure
