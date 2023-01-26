# Command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC, Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Import the sys module.

### Step 2:
Pass the filename as the first argument after the name of script.Open the file as sys.argv[1]

### Step 3:
Read the file using read() method

### Step 4:
Use split() method to split the file content into words.

### Step 5:
Use len() to find the total words.

### Step 6:
Run the program to determine the number of words in the file create



## PROGRAM:
```
#Developed by: S Kantha Sishanth
#Reference no: 22007660

import sys
count={}
a=sys.argv[1]
with open(a,'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word]=1
            else:
                count[word]+=1
print(count)
f.close()
```

### OUTPUT:

#### Text file:
!['output'](/out01.png)
#### Output:
!['output'](/out02.png)


## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
