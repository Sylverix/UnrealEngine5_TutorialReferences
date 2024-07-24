# Unreal Engine 5 Tutorial References
This repository contains a README file of `How-Tos` for Unreal Engine 5. As I'm learning Unreal Engine 5, I've created a pseudo-knowledge base of tutorials that are basic and easy to understand.

I decided to make this reference guide because I often find myself recreating the same items, objects, and actions in various learning projects. This is a work in progress, and I'll continue to update it with more tutorials featuring basic and potentially crucial information.

There will also be sections that I've custom-created based on my own experiments when trying to get things to work, especially when I haven't found any good YouTube tutorials regarding the topic. For example: `4. How-To: Add Sprint Animation Locomotion (WIP) (Photos Only ATM)`.

Please note that this README file is specifically tailored to work with the `Third Person Template` in the Unreal Engine launcher.

## (Optional Learning)
* YouTube Playlist containing visual blueprint scripting fundamentals: https://youtube.com/playlist?list=PL2A3wMhmbeAq3WOT7kQ0EGby1YMb0zj5_&si=GmllEo98pr5od-Qm

## 1. How-To: Add Input Mappings to Player, Add Camera Input, Add Movement Input, Add Jump Input
YouTube Video Tutorial: https://www.youtube.com/watch?v=Z9zEEY7dGaM&t=759s

## 2. How-To: Add Sprint Input
YouTube Video Tutorial: https://www.youtube.com/watch?v=Z9zEEY7dGaM&t=759s

## 3. How-To: Add Crouch Input
YouTube Video Tutorial: https://www.youtube.com/watch?v=Y8dZJtIvris&list=PLFuQoM4mOizQ89-INdN3eJv1P-r1tnCJM&index=2

## 4. How-To: Add Sprint Animation Locomotion (WIP) (Photos Only ATM)
Animation used: https://www.mixamo.com/#/?page=1&query=sprint&type=Motion%2CMotionPack
![image](https://github.com/user-attachments/assets/85dd83b3-08c7-46ca-9e2d-6eac3ae36ea9)

### Steps involving pictures at the moment:
*Step 1:*
To modify the base `Third Person` character to utilize a `Sprint` animation, go into the `Animation Blueprint` and add a new pin to the `Sequence` node. Then, create a new boolean variable called `IsSprinting`, drag it into the canvas as a `Set` node, and connect it to the new pin you've created in the `Sequence` node. Then, create a new float variable and call it `MaxWalkSpeed`. Drag `GroundSpeed` and `MaxWalkSpeed` into the canvas and add a `Greater Than` node. Connect the `GroundSpeed` varaible to the top pin of the `GreaterThan` node and connect the `MaxWalkSpeed` node to the bottom pin. Then, connect the output pin to the `IsSprinting` node. Basically, what we are saying is that if the current `GroundSpeed` is greater than the `MaxWalkSpeed`, then we are sprinting.
![image](https://github.com/user-attachments/assets/e16e4fce-6548-4d34-ad65-068795b18ca7)
![image](https://github.com/user-attachments/assets/10cc6bee-a86b-4e36-8435-8114cb9b7331)
![image](https://github.com/user-attachments/assets/cc4cdbbf-7721-4df5-b908-9aa293117fb8)
![image](https://github.com/user-attachments/assets/da0de004-4f3a-4ec0-857d-cdb52021e8df)
![image](https://github.com/user-attachments/assets/0445d8a4-893c-46c1-a450-f06216fd12ac)

