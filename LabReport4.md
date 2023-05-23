# Lab Report 4

## Logging into ieng6 ( Step 4 ) 

```$ ssh cs15lsp23mx@ieng6.ucsd.edu```

This would sign me into my account with the provided 
information see figure 1.1 


![figure 1.1](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/cb30db03-c7aa-479d-bef3-90b63f68f4a4)

I generated an ssh key so this will not prompt me for my password 

## Clone your fork of the repository from your Github account ( Step 5 )
```$ git clone https://github.com/ulises0516/lab7.git```

This would clone us into our git repository we forked previously.

![figure 1.2](https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/cf59dd92-40f7-4466-874f-f1d133120c3c)



```cd lab7``` before continuing onto next step. This image shows the information provided after cloning. 

## Run the tests, demonstrating that they fail ( step 6 )

```$ bash test.sh```

This would run the script to test the code you can also,however compile
```$ javac ListExamplesTests.java``` then ```$ java ListExamplesTests``` to show the errors of the tests.

![figure 1.3](<img width="527" alt="Screenshot 2023-05-22 at 4 38 13 PM" src="https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/8c50724e-4990-4190-8233-21cf4c7e31a0">)

## Edit the code file to fix the failing tests ( step 7 )

```vim ListExamples.java```

this will allow you to enter vim to edit the code see figure 1.4 to see how it looks like and on the right path.

![figure 1.4](<img width="667" alt="Screenshot 2023-05-22 at 4 11 00 PM" src="https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/f4d4c80f-d18c-4943-911b-82fcb72d1df5">)

1. ```/``` 
2. type **index1**
3. ```<return>```
4. type "n" 10 times 
5.  ```<escape>```
6.  ```< right arrow key> <right arrow key> <right arroy key>  <right arrow key> <right arrow key>```
7.  press **x**
8.  press **i** to go into index mode
9.  press **2**
10.  ```escape```
11.  ```:```wq
12.  ```<enter>```

These sequence of steps will fix the error in the code.

**SIDE NOTE - Extra information on what the steps do** 

The frst step is a the default character that will alow you search for a word. The 4th step is basically says "search for the next occurence of the word". The 5th step is common to escape current mode. the 8th mode is a common mode called index mode which allows you to type follows your cursor. Then 10th step is to escape the current mode which is index mode. The 11 step essentially says "save then quit".

## Run the Tests, demonstrating they now succeed (step 8)

```$ bash test.sh```

This should now display that the tests succeed see figure 1.5 for what the mesage should show 

![figure 1.5](<img width="334" alt="Screenshot 2023-05-22 at 4 14 16 PM" src="https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/de6ab616-74c3-4c68-8d4d-140bcc978d80">)

## Commit and push resulting to change to your github account ( step 9)

Complete generating ssh keys for github for a smooth process 

```$ git add ListExamples.java```
```$ git commit -m "<enter message of your choosing>"```
```$ git push git@github.com:ulises0516/lab7.git```

Enter these commands in the sequence. However for ```$ git push``` put your ssh key from github under the code section then the section ssh. This will display your own if you completed ssh keys for github correctly. See figure 1.6 for a what a successful commit and push looks like.

![figure 1.6](<img width="665" alt="Screenshot 2023-05-22 at 4 42 17 PM" src="https://github.com/ulises0516/cse15l-lab-reports/assets/125671517/1646958e-af88-43ac-8b69-283e7d120b31">)

**Side Note**

You can press tab after typing ListE... and it would autofill the word ListExamples.java to be more quick.
























