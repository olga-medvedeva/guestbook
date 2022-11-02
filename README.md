# Small project using Go

### A service that receives data from the user, writes it to a file and displays it on an HTML page;

Service has following functions:

- When user gets to [http://localhost:8080/guestbook](http://localhost:8080/guestbook) (img 1) it displays all of the information that was read from **signatures.txt** file. 
  When project starts, there are 4 lines in the **signatures.txt** file:
```
First signature
Second signature
Third signature
Forth signature
```

- If user wants to add his signature this can be done using the link * *Add your signature* *. This link gets user to a page [http://localhost:8080/guestbook/new](http://localhost:8080/guestbook/new) (img 2) which takes the input information, creates new signature throw http://localhost:8080/guestbook/create (which user doesn't see), appends it in **signatures.txt** and redirects back to [http://localhost:8080/guestbook](http://localhost:8080/guestbook) (img 3) where new information already displayed.
  
  After adding fifth signature **signatures.txt** looks as this:
```
First signature
Second signature
Third signature
Forth signature
5th signature
```

![1](https://user-images.githubusercontent.com/90202470/199536817-d9849291-4e89-4ad4-9227-70ffb9e0cdc9.jpg)
<p align="center">[1]</p>


![2](https://user-images.githubusercontent.com/90202470/199536907-8b08b85d-21f9-425a-9290-528a7c9e6b3f.jpg)
<p align="center">[2]</p>

![3](https://user-images.githubusercontent.com/90202470/199536950-2221111b-6fde-4db7-907f-983cc7c982a9.jpg)
<p align="center">[3]</p>
