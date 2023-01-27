# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 

### Step 1:

Import the sys module.
### Step 2:

Pass the filename as the first argument after the name of script.Open the file as sys.argv[1]
### Step 3:

Read the file using read() method.
### Step 4:

Use split() method to split the file content into words.
### Step 5:

Use len() to find the total words.
### Step 6:

Run the program to determine the number of words in the file created.

## PROGRAM:
```
DEVELOPED BY : SARGURU K
REF NO : 22002828

import sys
d={}
f=open(sys.argv[1],"r")
for line in f:
    l=line.split(" ")
    for word in l:
        if word not in d:
            d[word]=1
        else:
            d[word]+=1
print(d)
f.close()
```

### OUTPUT:
![1](./scr1.png)

![2](./scr2.png)






## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
