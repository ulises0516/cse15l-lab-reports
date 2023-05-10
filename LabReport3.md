# Lab Report 3
--- 
  ## First option of grep (*grep -c*)
  
  ---
  Example 1
  
  
  ``` 
     $ find technical/ > find-results.txt
     $ grep -c "preface" find-results.txt
  ```
  --- 
  Example 2
  
  
  ```
    $ grep -c "treat" technical/biomed/1468-6708-3-10.txt
  ```
  ---
  
  **How it Works(Example 1)** 
  
  The first line in example 1 starts searching from techincal/ and finds all the directories. 
  and "finds" the files and directoreis essentially a walking file hiearchy. The. 
  second line with the option "-c" counts the amount of lines that matches a pattern. 
  which I gave "preface" in the find-results.txt. This would output 1 as the result.
  
  **How its Works(Example 2)**
  
  The line searches through the file to match the pattern "treat" and it outputs ```32``` indicating. 
  that there were 32 lines that had the word "treat"
  
  **How its Useful**
  
  This command breaks narrows the focus of essentially the ``` $ wc ``` command which displays. 
  the character words and amount of lines. ```$ grep -c```  just displays the amount of lines. This
  is useful if just want to display only the count of lines eliminating clutter in your command line.
 
 --- 
## Second option of grep (*grep -i*)
 ---
    Example 1
    $ grep -i "research" technical/biomed/1468-6708-3-10.txt
    Example 2
    $ grep -i "ssc" technical/biomed/1471-213X-1-1.txt
    ---
      **How it Works** 
      The line searches through the file to match "ssc" however the -i  makes it so searches. 
      case insensitive. 
     
