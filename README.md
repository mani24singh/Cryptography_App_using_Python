# Cryptography App using Python
Developing a cryptography app in python to encrypt and decrypt a normal text message

## Install the cryptography package:
- !pip install cryptography
- Import fernet module from cryptography.fernet package
- from cryptography.fernet import Fernet

## Functions used:
1. **generatePassKey:** 
     - This function is used to generate a key and save it in a file(.key extension)
     - Key is generated by using a generate_key() function which is inside the fernet module.
   - And it is saved in a file using file handling
2. **getMyKey:**
     - This function is used to get the key which is saved in the file and return the key.
     - Here the file is read using file handling
3.	**getContentFromUser:**
     - It is a simple function which returns a string which is given by the user, using the input()
4.	**encryptMessage:**
    - This function takes a parameter called message_normal which needs to be encrypted
    - First, it calls the getMyKey function to get the key value from the file
    - Now an object is created using the key called k
    - And then the message is encrypted using encrypt(message_normal)
    - At last it returns the encrypted message
5.	**decryptMessage:**
    - This function takes a parameter called message_secret which needs to be decrypted
    - First, it calls the getMyKey function to get the key value from the file
    - Now an object is created using the key called k
    - And then the message_secret is decrypted using decrypt(message_secret)
    - At last it returns the decrypted message

## Setting up path:
### How to install and write python codes?
- Go to www.python.org
- Choose the latest python version suitable for your user interface  machine (mac,windows,liinux etc).
- It will be installed and in your machines as either terminal or command line or python.
- To check python is installed or not , Type print command in command line & check the output. While other easier way of checking is using anaconda as described below.
- Other way of using python is using google colab (Go to Google colab in google) and run python using your machine (including mobile phones).

### Anaconda:-  
- Go to  www.anacond.com  & download.
- It is like a  bundle that is downloaded with python and along with famous libraries. It is preferred by most data scientists.
- Find anaconda navigator in your machine and open it. You will find different visualizing tools like jupyter lab, jupyter notebook, spyder, orange3, vs code, rstudio, vs code. We need this bundle for jupyter notebook.

### Jupyter NoteBook:- 
- It is a web-based interactive portal that allows us to give input and see the output then and there in a clean and clear manner.
- How to start programming in Jupyter NoteBook:-
   - Step1: Open Anaconda navigator and select Jupyter NoteBook & click launch.
   - Step2: Create a new folder and rename it.
   - Step3: Go inside the folder and go into new options and select python 3.
   - Step4: Name the python notebook.
   - Step5: Type the code in the cell. And to run the code press shift+enter
 
 ## Modules & Packages:- 
- Modules are nothing but a file (with .py extension) which we can import into a particular program
- Group of modules(python files) is known as package 
### Pypi.org :
- pypi.org is a website where we all can get different libraries which we can use for a different purpose.
- How to install a library from pypi.org
   - Go to pypi.org.
   - Search for a library according to your need.
   - Copy the text which says “pip install library name”.
   - In Jupyter notebook type “!” and paste the content and run the cell.
   - The library is installed on the local machine
### How to create our module:
   - Modules are created using a special keyword which is only for Jupyter notebook and Google Colab.
   - Create a module by
       - %%writefile ModuleName.py
       - #And write a python code
   - Import the module in another program and use the functions inside the module
      - import ModuleName
      - ModuleName.FunctionName()
### How to create Package:-
- Make a folder and rename it(That is your package name)
- Now we can import a module through the package, like
   - from packageName import moduleName
