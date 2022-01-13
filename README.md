# Steganography using LSB

**_Hide text messages in images_**

(**TL;DR :** _This program can hide a text message in an image, which can only
be decoded by this program only._)

### Requirements
  
  Make sure all the libraries must be installed and import
  
  ```console
    import cv2
    import numpy as np 
    import types 
    import matplotlib.pyplot as plt 
    import matplotlib.image as mpimg 
  ```


1. Three step for Steganography using LSB
  - **KeySpace**
  - **Encoding** 
  - **Decoding**

### KeySpace

  KeySpace is class when we create object we need three argument while creating the class
    
    1. 'start_x' - Starting position of column pixel 
    2. 'start_y' - Starting position of row pixel 
    3. 'key' - This is for how many pixel we skip 
    
    Note - This KeySpace is private to sender as well as reciever


### Encoding

  'encodeText' is method will take two argument first are 'Image_path' and 'KeySpace'
  
  ```console
    pepper.png (RGB Image)
    cameraman.png (Grayscale Image)
  ```
  
  **_You can also use any image you want as carrier, but make sure to add them
  into "root_folder"**
  
  Now this will ask you to enter the text which you want to hide inside that
  image.
  Then it will encode your text in the image and save as 
  
  
  ```console
    original_file_name+"_stego."+filetype
  ```
  in 'root_folder'
  
  ![image](https://user-images.githubusercontent.com/55941465/149313459-9f5573d8-7069-49f4-aae5-ce71e73ae77e.png)

### Decoding

  'decodeText' is a method will take two argument first are 'encoded_image_path' that is present in 'root_folder' and same 'KeySpace'
  use by sender.
  
  ![image](https://user-images.githubusercontent.com/55941465/149316474-5e5d7844-3ef1-44ff-9003-a2ae782d4f61.png)
  
  
##

## Now let's see what changed visually:

### Pepper:

![image](https://user-images.githubusercontent.com/55941465/149318168-075e9ce8-0a98-4074-a492-285c81fed708.png)

### Cameraman

![image](https://user-images.githubusercontent.com/55941465/149318249-3092798f-1c25-42ec-85e1-269547d28d4c.png)




  
  
  
  
