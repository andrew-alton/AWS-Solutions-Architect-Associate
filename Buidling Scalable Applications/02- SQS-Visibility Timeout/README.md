## Challenge

When consumer receiving a message from the queue , the message still remains in the queue and is not deleted.
What is the challenge if the message is deleted?

![My Image](images/image1.png)

##  Visibility Timeout

When consumer receives a message from the queue, the message still remains in the queue and is not deleted. However it remains in hiden satate for specific interval and can be 
deleted by consumer once it has completed procceing.

![My Image](images/image2.png)