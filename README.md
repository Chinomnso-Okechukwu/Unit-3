# Unit-3

Contents
--------
  1. [Planning](#planning)
  1. [Design](#design)
  1. [Development](#development)
  1. [Evaluation](#evaluation)
  
## Planning
### Definition of problem
The client for this application is Hassan Ali, a lover of perfumes. He has so much perfumes of different brands, sizes and content. They all smell soo good and sometimes he can spend lots of minutes thinking of what perfume to use for heading out for school. This action comes at his expense because he usually misses breakfast and comes late for his first period classes. Hassan has also found it hard to account for his numerous perfumes. He tends to lose a lot of them and it has become a hell of a job to organize his perfumes. 

### Proposed solution
I am going to create an application that helps Hassan organize his perfumes in the form of an inventory. On opening the application, there would be a feature that informs him on the recommended perfume to use that particular day. This application will also be only accessible to him.
I will make use of the Python programming language to develop this application. My justification for using Python is due to its ability to give better results, agility and user experience to the customers. GitHub along with many other portals have positioned Python in top 10 languages for mobile application development. What makes Python easy to understand is its unmistakable, natural and basic syntax that looks like English. Such features make Python the best choice for amateurs.[1]

### Success Criteria
1. Application must be secure. No other person should be able to gain unauthorized access.
2. There should be a recommended perfume for that season when the client opens the application.
3. Click system to check out or use perfume and informs client when perfume was last used.
4. Client should be able to create or add a new perfume to his inventory.
5. Client should be able to delete or remove an existing perfume from his inventory.
6. Client should be able to edit a perfume in his inventory.
7. Application should be visually pleasing.
8. Application should be easy to use.

## Design

## Development

```.py
mysecretpass = '2'
user = 'H'

    def trylogin(self):
        # 1. get the name
        # 2. get the password
        # 3. compare name entered and stored
        # 4. same with password
        nameEntered = self.email_in.text()
        passEntered = self.pssword_in.text()
        print(nameEntered)
        print(passEntered)

        self.email_in.setStyleSheet("border: none")
        self.pssword_in.setStyleSheet("border: none")

        if nameEntered != user and passEntered != mysecretpass:
            self.email_in.setStyleSheet("border: 2px solid red")
            self.pssword_in.setStyleSheet("border: 2px solid red")
            print('1')
        elif nameEntered != user:
            self.email_in.setStyleSheet("border: 2px solid red")
            print('2')
        elif passEntered != mysecretpass:
            self.pssword_in.setStyleSheet("border: 2px solid red")
            print('3')
        else:
            self.email_in.setStyleSheet("border: 2px solid green")
            self.pssword_in.setStyleSheet("border: 2px solid green")
            print('passwords okay')
            self.done(0)
```
The snippet of the code shows the steps for logging in. Since the application is to be accessed by only one person, I conversed with my client and had a password and username fixed with him. The program is already inbuilt with a correct password and username. Any person ,including my client, trying to access the app has to input a username and password.
The if statement is used to compare the values inputed by a person and the inbuilt password and username. The borders of the input boxes are white initially. If one or both of the values are wrong, the border(s) of the wrong input box becomes red. If both are correct, it is green and login is successful. The use of 'if' statements here shows my algorithmic thinking. 

### References
[1] Retrieved from https://topofstacksoftware.com/2019/01/09/10-best-programming-languages-for-mobile-app-development/ on 15th February 2020.
