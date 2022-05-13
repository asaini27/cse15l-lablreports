## THIS IS LAB REPORT 3 - WEEK 6

# PART 1: Streamlining ssh Configuration

The following image shows my config file:

<img width="739" alt="Screenshot 2022-05-11 at 2 12 08 AM" src="https://user-images.githubusercontent.com/103229052/168348136-182a039e-29f4-4b8b-97b3-120e72b9fa8a.png">

After completing config, it makes it easier to log in to the remote computer

<img width="1032" alt="Screenshot 2022-05-08 at 9 34 06 PM" src="https://user-images.githubusercontent.com/103229052/168349598-1176acfc-e2bc-4951-a6f7-0a37d1047651.png">

It also makes the process of copying a file easier, in the following image I am copying the file forReport3.java:

<img width="650" alt="Screenshot 2022-05-11 at 2 18 43 AM" src="https://user-images.githubusercontent.com/103229052/168352772-11d70d62-6a40-40e8-90d7-c26c7f06c482.png">


# PART 2: Setup Github Access from ieng6

This is my public key on github:

<img width="1295" alt="Screenshot 2022-05-13 at 11 55 54 AM" src="https://user-images.githubusercontent.com/103229052/168358625-e2bcbd75-dd8d-4e52-9de1-d208fa87bf75.png">

The following screenshot is of the ssh file opened on VScode which shows my private (id_rsa) and public (id_rsa.pub) key:

<img width="650" alt="Screenshot 2022-05-11 at 2 12 26 AM" src="https://user-images.githubusercontent.com/103229052/168365082-1709c48d-1cde-40d4-b224-ee26fd7d9b1c.png">

The image below depicts the result of using git commands while logged in ssh:

<img width="695" alt="Screenshot 2022-05-12 at 7 34 07 PM" src="https://user-images.githubusercontent.com/103229052/168368128-8a30aae9-8132-48e5-8f9e-b140762d87b4.png">

[LINK TO THE UPDATE MADE USING GIT COMMANDS ON TERMINAL](https://github.com/asaini27/markdown-parser/commit/64a38cf2b9d7af2b8bb75efe757543ac724f7857)


# PART 3: Copy whole directories with scp -r

Copying the markdown-parser directory to ieng6:

<img width="977" alt="Screenshot 2022-05-12 at 7 39 02 PM" src="https://user-images.githubusercontent.com/103229052/168373604-574e8253-1d43-4c95-94f6-7698923ae629.png">

<img width="1223" alt="Screenshot 2022-05-12 at 7 39 18 PM" src="https://user-images.githubusercontent.com/103229052/168373640-585cc30c-124b-4e73-8cae-b6fc2aa62e7d.png">

<img width="685" alt="Screenshot 2022-05-12 at 7 40 06 PM" src="https://user-images.githubusercontent.com/103229052/168373774-dfbc6e23-7e39-4899-ae17-3bc932ee3dc7.png">

Now while being logged in ieng6, compiling and running my tests:

<img width="676" alt="Screenshot 2022-05-13 at 10 27 50 AM" src="https://user-images.githubusercontent.com/103229052/168373967-87c2e80b-0de9-4aa2-8ba0-6df71fad6d53.png">

Now combining scp, ;, and ssh to copy the whole directory and run the tests in one line, I get this:

<img width="1214" alt="Screenshot 2022-05-13 at 12 33 29 PM" src="https://user-images.githubusercontent.com/103229052/168377292-3d3e0094-14d2-49e1-8b22-394c63a9f5f4.png">

<img width="1222" alt="Screenshot 2022-05-13 at 12 33 52 PM" src="https://user-images.githubusercontent.com/103229052/168377315-0d93b45e-6df1-4589-bb20-a893d22b095f.png">

<img width="1210" alt="Screenshot 2022-05-13 at 12 34 06 PM" src="https://user-images.githubusercontent.com/103229052/168377365-27a420d0-bd53-45eb-b1fb-ff36e32d595f.png">






