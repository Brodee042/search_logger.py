## Example Requests:
> with open("request.txt", "w") as request:  
>‎ ‎ ‎ ‎ ‎ request.write("w 1, 2, 3, 4")

> with open("request.txt", "w") as request:  
>     request.write("d")

> with open("request.txt", "w") as request:  
>     request.write("c")

  Overall, their are 3 commands that one can use for the search_logger.py microservice, those being write, delete, and copy. Write requires you to
write inside request.txt a request that starts with "w ", which tells the computer that anything that comes after should become a new entry in log.txt.
The second comand is called when their is a singular "d" inside request.txt. This deletes the last entry within log.txt. The third and most important
function is copy, which makes is so that a copy of log.txt is made on response.txt, which the user can then extract info from and interact with. All of 
this ensures the seperation of the log.txt file from the developer, helping to make this a microservice.


## Example Response:
> with open("response.txt", "r") as response:  
>     print(response.read())

  This only comes in to play after a user has sent a request for a copy via request.txt. Once this is done, the program prompty creates a copy of log.txt
on response.txt, which you can then read, interact with among other things. This ensures that the user does not need to, and cannot interact with log.txt
directly. Below is a UML example of the response part of the program.


![Screenshot 2025-05-19 at 18-50-53 Untitled document - Google Docs](https://github.com/user-attachments/assets/e6f9b446-68ed-4138-91a8-84279093d32a)
