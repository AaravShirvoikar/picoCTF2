![Screenshot from 2023-02-19 15-11-22](https://user-images.githubusercontent.com/115702866/219940464-aeb8ff77-1d5e-46ff-808b-0fd6aafc6554.png)

First, I tried to run the progam and I got the following error.

```t
aarav@aarav-Inspiron-3584:~/Downloads$ ./vuln
bash: ./vuln: Permission denied
```

I changed the permissions of the file and tried to run it but I got a segmentation fault error.

```t
aarav@aarav-Inspiron-3584:~/Downloads$ chmod +x vuln
aarav@aarav-Inspiron-3584:~/Downloads$ ./vuln
Segmentation fault (core dumped)
```

I ran the following command and found out that the program is an echo server requests an inout string, slightly modifies it and outputs it.

```t
aarav@aarav-Inspiron-3584:~/Downloads$ nc mercury.picoctf.net 37289
WeLcOmE To mY EcHo sErVeR!
bruh
BrUh
no i dont want that
No i dOnT WaNt tHaT
```





