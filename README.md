The Reverse Hash Application
============================

This application uses a very simple brute force attack to 
"reverse" an MD5 hash.  It is really not reversing the hash
at all as that would be impossible.  Instead it knows that 
the original pre hash text was a lower case character string with 
exactly two characters.

So the application uses two nested loops and tests all 
26*26 combinations of two lower case letters, and computes the
hashes of those values and checks to see if the computed hash
matches.


This is a lesson in how easy it is to crack short passwords
with a limited alphabet.  While this works well to crack 
very short passwords it is not practical as password 
length grows.

A more sophisticated attack ti reverse hashes which uses a 
lot of storage to pre-compute lots of hashes and look them up
quickly is called "Rainbow Tables".  This tiny application
is *not* using a Rainbow Table approach.

Website View:

![image](https://user-images.githubusercontent.com/64192420/110159361-cedd7e00-7e14-11eb-939c-b5cc75bdde6c.png)

Makecode:
![image](https://user-images.githubusercontent.com/64192420/110159438-e7e62f00-7e14-11eb-8190-347daee3f05d.png)

