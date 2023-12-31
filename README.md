# copy-file
## AIM:
To write a python program for copying the contents from one file to another file.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
### Step 1:
Open the Source File for Reading:

Use the open function with the 'r' mode to open the source file ('myfile1.txt') for reading. Assign the file object to the variable source.
### Step 2: 
Read Content from Source File:

Use the read method on the source file object to read the content of the source file. Assign the content to the variable content.
### Step 3: 
Open the Destination File for Writing:

Use the open function with the 'w' mode to open the destination file ('myfile2.txt') for writing. Assign the file object to the variable destination.
### Step 4:  
Write Content to Destination File:

Use the write method on the destination file object to write the content to the destination file.
### Step 5: 
Print Success Message:

If the file copy operation is successful without errors, print "File copied successfully!".
### Step 6: 
Read and Print Copied Content:

Open the destination file ('myfile2..txt') for reading. Read the content from the destination file and assign it to the variable data. Print the copied content using print(f"Copied content:\n{data}").
## PROGRAM:
```
# Program to copy file 1 contents to file 2
# Developed By :K Kesava sai
# Register Number : 212223230105
try:
    with open("myfile1.txt", 'r') as source:
        content = source.read()

    with open("myfile2.txt", 'w') as destination:
        destination.write(content)

    print("File copied successfully!")
    
    with open("myfile2.txt",'r') as fp:
        data = fp.read()
        
    print(f"Copied content:\n{data}")

except FileNotFoundError:
    print("One or both files not found.")
except Exception as e:
    print(f"An error occurred: {str(e)}")
```

### OUTPUT:
![image](https://github.com/Kesavasai20/copy-file/assets/138849303/fd64c07b-6a35-4a55-a6ee-1b76170ce1ae)
![image](https://github.com/Kesavasai20/copy-file/assets/138849303/4f0853b2-e47b-45d5-b3a8-a1cddb92417d)
![image](https://github.com/Kesavasai20/copy-file/assets/138849303/aa402df3-7b8c-4991-aff6-6c0c84d95259)
## RESULT:
Thus the program is written to copy the contents from one file to another file.
