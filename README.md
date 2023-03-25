# CSerialIO_VS2022 This is a Visual C++ Project originally created by tojine on Code Project.

According to the author:

"It implements the serial communication using a thread to enable data being captured anytime, 
you just handle the event of READ/WRITE/OPEN/CLOSE via inheriting this class"

Link: https://www.codeproject.com/Articles/99375/CSerialIO-A-Useful-and-Simple-Serial-Communication

Download: Demo version

This implements two way serial communication which allows user to select baud rate and com port.
There appears to be a bug in the demo: the user selected baud rate wasn't being used.
Instead it was stuck at default 115200 baud.

I fixed this bug and substituted a CEdit box instead of a List box to dsiplay incoming text.
The incoming text is read in and stored in a buffer until a carriage return is received,
at which point it is displayed in the CEdit box.

I found the List box approach to be less useful than a CEdit box.

I hope you find this useful - Jim
