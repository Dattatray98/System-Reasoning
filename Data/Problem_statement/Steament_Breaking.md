# Systems Reasoning with NLP and Generative AI

## What should use 
 1. Big story (Novel):
    - Novel-1 : In search of the castaways
    - Novel-2 : The Count of Monte Cristo

 2. Small story (Backstory):
    - train.csv
    - test.csv

 3. pathway (important tool):
    - for storing the stories.

 4. LLM (AI helper):
    - for answering 


## Where to use 
 1. Big Story 
    - First thing that program reads.

 2. Pathway
    - where story is too big
    - store story in pieces here 
    - retrive story pieces from here 
    - use semmantic search for retriving    

 3. small story
    - use it after reading big story
    - break into small points

 4. LLM
    - use only to check
    - Not to write stories 
    - Not to chat


## How to use these 
 1. Use of Big story
    - System reads the full story

 2. Use of pathway
    - Cut big story into small parts and store.
    - Because the big story is too big 
    - Pathway remembers everything neatly.
    - Each story chunk should contain :
      > Story test
      > piece number
      > book name
      > name of character if possible

 3. Use small story (Backstory)
    - Read backstory.
    - Backstory is in the content column in csv
    - break it into points.

 4. Use Pathway again
    - For each point
      > Ask pathway : Give me story parts about this person
      > Pathway gives : early part, middle part, late part
      > Now you will see the full life
    
 5. Use LLM (AI helper)
    - Ask a small question to LLM
      > use chain-of-thought prompting, claim decomposition, and confidence scoring.
    - LLM answers :
      > TRUE
      > FLASE
      > NOT CLEAR
    - do this for all points

 6. Final decision
    - If any strong FALSE --> answer 0
    - Else --> answer 1

 7. Save Answer
    - Write in file
      > Story Id
      > Book Name
      > Char
      > 1 or 0
      > small reason
    

