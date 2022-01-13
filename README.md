# Steganography using LSB

**_Hide text messages in images_**

(**TL;DR :** _This program can hide a text message in an image, which can only
be decoded by this program only._)


### Three step for Steganography using LSB
  - **KeySpace**
  - **Encoding** 
  - **Decoding**

### KeySpace

  KeySpace is data structure that contain keys.
  
  We need three argument from user while creating the object
   
    'key' - Key contain Alpha, Numeric and Symbol
    
    Note - This KeySpace is private to sender as well as reciever


### Encoding

  'encodeText' is method which is used for ecoding that will take two argument first are 'Image_path' and 'KeySpace'
  
  ```console
    pepper.png (RGB Image)
    cameraman.png (Grayscale Image)
  ```
  
  **You can also use any image you want as carrier, but make sure to add them
  into "root_folder"**
  
  Now this will ask you to enter the text which you want to hide inside that
  image.
  Then it will encode your text in the image and save in 'root_folder' as
  
  ```console
    original_file_name+"_stego."+filetype
  ```
  
  ![image](https://user-images.githubusercontent.com/55941465/149354297-be063e89-47cd-4932-85f1-e412fd98f839.png)

### Decoding

  'decodeText' is a method will take two argument first are 'encoded_image_path' that is present in 'root_folder' and same 'KeySpace'
  use by sender.
  
  ![image](https://user-images.githubusercontent.com/55941465/149354396-b1ca53af-4e24-42a6-83ac-3b62ce05fcb0.png)
 




  
  
  
  
