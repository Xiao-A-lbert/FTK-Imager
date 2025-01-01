# FTK Imager

<h2>Description</h2>
In this Digital Forensics task, I explore FTK Imager where I examine a sample hard drive of a deleted photo, create a disk image, and captured my VM's memory. 

<h2>Languages and Utilities Used</h2>

- <b>FTK Imager</b>
- <b>Powershell</b>

<h2>Environments Used </h2>

- <b>Windows 10 Enterprise</b> 

<br />
<br />
After creating a virtual drive mounted to my windows vm desktop and populating it with a sample user file, I added the evidence drice to FTK Imager and navigated to the user's camera roll showing a cat.jpg.

![1) investigating sample hard drive](https://github.com/user-attachments/assets/59e5aae3-fc4c-40fe-8cc9-569a53aed5ee)

<br />
<br />
In the cmd, I deleted the cat.jpg. 

![2) deleting cat phot](https://github.com/user-attachments/assets/f482fc63-fdf6-4f1a-82ca-eaf99ec2a50d)

<br />
<br />  
Re-uploading the evidence drive, I can see the same cat photo being shown as deleted from the drive. 

![3) cat pic is still there](https://github.com/user-attachments/assets/68da5fce-bca0-40e6-b066-e1396c9fe212)

<br />
<br />
To create an disk image, go to File>Create Disk Image.

![4) create disk image](https://github.com/user-attachments/assets/263fcefd-4c2c-473f-ac9a-e9f381765ba3)

<br />
<br />
Select Physical Drive.  

![5) physical](https://github.com/user-attachments/assets/d7330afb-b03f-492f-8673-97eec66f4d53)

<br />
<br />
Select Add>E01 which is a forensic image file format used to create bit-by-bit copies of digital storage devices, preserving original data for analysis while supporting compression, metadata inclusion, and integrity verification through checksums and hashes.

![6) add](https://github.com/user-attachments/assets/9a7975aa-7536-4264-a6a8-76dad13094a4)

<br />
<br />  
I enter the Evidence Item information includeing a case number with the date, an example evidence number, a unique description, examiner, and other notes. 

![7) info](https://github.com/user-attachments/assets/e720a24a-3ef3-4832-8642-b68469585196)

<br />
<br />  
Then select an image destination, in this example I set it to my Desktop. 

![8) saving](https://github.com/user-attachments/assets/fc86cd5b-aca3-4a20-b82a-41390e5a20ea)

<br />
<br />
To capture memory, select File>Capture Memory.

![9) capture memory](https://github.com/user-attachments/assets/c2ca0dfd-07d2-4ea2-94c4-bddaf4639213)

<br />
<br />  
I selected my desktop as a destination and the file name for capturing my windows 10 vm. 

![10) mem cap](https://github.com/user-attachments/assets/fad9bfca-62d5-4bd3-960e-133b422a2df5)

<br />
<br />  
I ran powershell to generate a sha256 hash of the memory capture. 

![11) sha256 mem](https://github.com/user-attachments/assets/d6524969-e752-45cc-9735-0e14eb03867d)

<br />
<br />
