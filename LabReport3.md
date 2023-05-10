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
## 2nd option of grep (*grep -i*)
  
  ---
  Example 1
  ```
  $ grep -i "gaba" technical/biomed/1471-213X-1-1.txt
  ```
  ---
  Example 2
  ```
  $ grep -i "ssc" technical/biomed/1471-213X-1-1.txt
  ```
  
  **How it works(example 1)**
  
   The command grep -i searches the text file "gaba" but in a case insensitive way.
   The output for this command was
   ```
   the inhibitory neurotransmitter γ-amino butyric acid (GABA)
        Gad2 respectively [ 1, 2, 3]. GABA
        Early in CNS development, GABA can modulate neuron
        12, 13, 14]. In some classes of neural progenitors GABA
        demonstrated that GABA acts in the developing neocortex to
        postnatal development, normal GABAergic input is required
        addition to these functions in the developing CNS, GABA
        of GABA-mediated signals in the normal development and
        the β3 subunit of the GABA 
        GABA-mediated signaling in the development of a non-neural
        of GABA [ 30, 31]. During embryogenesis,
        production of GAD proteins and the synthesis of GABA in the
        the mouse embryo, suggesting a potential role for GABA
        Our interest in the role of GABA signaling in developing
        Gad1 and the β3 GABA 
        21, 22]. The genetic data strongly suggest that GABA acts
        through GABA 
        examine the expression pattern of GABA receptors in the
        Expression of GABA receptor subunits in adjacent tissues
        signals mediated by GABA in these structures and
        and GABA in the development of non-neural tissues than was
  ```
   
  **How it works(example 2**
   
   The command grep -i searches the text file for "scc" ignoring case sensitivity.
   The output for this command was 
   ```
    to the probe overnight in 50% formamide, 5X SSC (pH 5.0),
        at high stringency in prewarmed 50% formamide, 5X SSC, 1%
        were washed in three changes of 50% formamide, 2X SSC pH5.0
   ```
   
   
   **How is it useful** 
   
   It can be annoying to write all caps out everyone knows this but the most useful thing is 
   it elimnates the any outlier you may miss if you are seraching for a word "The" or "the 
   ``` grep -i ``` will displays both.
   
   
   ---
   

   
   

    

     
