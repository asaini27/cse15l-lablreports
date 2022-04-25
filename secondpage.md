## THIS IS WEEK 4 LAB REPORT 2 

*BY ADITYA SAINI*

## ISSUE 1

[ISSUE 1](https://github.com/asaini27/markdown-parser/blob/main/file2.md)

*TRYING TO GET THE LINK WHEN IT IS IN THE FORMAT:*
[NAME]!WEBSITE LINK?

<img width="1279" alt="Screenshot 2022-04-24 at 9 14 08 PM" src="https://user-images.githubusercontent.com/103229052/165019787-aac98091-0c3c-4595-ba9e-66e6e2ad88f5.png">

## ISSUE 1 FIXED
<img width="1279" alt="Screenshot 2022-04-24 at 9 14 08 PM" src="https://user-images.githubusercontent.com/103229052/165019884-2b761b59-9f69-4f04-bda0-532185b1994b.png">

The markdown file with errors is the failure inducing input. The failure inducing input is the one which basically caused the bug, here it is '!' and '?' instead of using the "(" and ")" around the website name. The bug is a string out of bounds excpetion and the symptom is an undesired output. 

## ISSUE 2 

[ISSUE 2](https://github.com/asaini27/markdown-parser/blob/main/file4.md)

*TRYING TO GET THE LINK WHEN IT IS IN THE FORMAT:*
(NAME)[WEBSITE LINK]
<img width="1287" alt="Screenshot 2022-04-24 at 9 15 18 PM" src="https://user-images.githubusercontent.com/103229052/165020090-9e2bd505-061c-415f-9f6f-fccfc187a5b2.png">

## ISSUE 2 FIXED
<img width="1312" alt="Screenshot 2022-04-24 at 9 18 57 PM" src="https://user-images.githubusercontent.com/103229052/165020233-c8ab0f94-7e2d-4a43-b72d-7a86310651b8.png">

In this the failure induced input refers to the use of "(" and ")" for the name of the link and '[]' for the website link. This failure inducing input lead to the bug ie the output is a broken link which doesn't work, and the symptom was again an undesired output. 

## ISSUE 3

[ISSUE 3](https://github.com/asaini27/markdown-parser/blob/main/file5.md)

*TRYING TO GET THE LINK WHEN IT IS IN THE FORMAT:*
[NAME]!* WEBSITE LINK *!
<img width="1273" alt="Screenshot 2022-04-24 at 9 22 28 PM" src="https://user-images.githubusercontent.com/103229052/165020596-2fc8ad00-f4ca-4f3b-93be-1d39732d0b88.png">
<img width="1359" alt="Screenshot 2022-04-24 at 9 22 37 PM" src="https://user-images.githubusercontent.com/103229052/165020617-16f62b1c-c56d-45a3-b0e7-9a7d69fd3030.png">

## ISSUE 3 FIXED
<img width="1255" alt="Screenshot 2022-04-24 at 9 23 58 PM" src="https://user-images.githubusercontent.com/103229052/165020718-1fa01421-130d-42c0-8cdc-001e64058cd4.png">

In this issue the use of "/*" and "*/" instead of "()" around the website link caused an error. The bug was a string out of bounds excpetion and the 
symptom was an undesired output rather than a properly functioning link. 
