<h1> Ventoy - Insallation and Demonstration </h1>

<h2>Description</h2>

Project consists of a simple installation of a program named Ventoy on a USB device. Typically, when you want to create a bootable device, the entire space of the drive is utilized for that purpose. Ventoy alleviates that problem with creating an EFI directory on the bootable drive first then allowing you to select which ISO you would like to run on the device. The only issue I have had with this is that Secure Boot needs to be disabled or else Ventoy will be flagged exploit. Otherwise, Ventoy is perfect for me to have multiple versions of ISOs on a single drive.

In this tutorial, we will be installing Ventoy on the USB and test a Windows 10.iso image to verify it's usability.

<h2> Utilities Used </h2>

- <b>32GB USB Drive</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Download the latest version of <a href="https://www.ventoy.net/en/download.html">Ventoy</a>: <br/>
<img src="https://i.imgur.com/Mkbe8U3.png" height="80%" width="80%" />
<br />
<br />
Link will direct you to Github, select Windows.zip  <br/>
<img src="https://i.imgur.com/DDdB1JJ.png" title="source: imgur.com" />
<br />
<br />
Go ahead and extract the file's contents to a folder: <br/>
<img src="https://i.imgur.com/arQJfjP.png" title="source: imgur.com" /></a>
<br />
<br />
Once extracted, open Ventoy2Disk X86 and connect your USB:<br/>
<img src="https://i.imgur.com/mUvuXQQ.png" title="source: imgur.com" /></a>
<br />
<br />
Select your device and click install. (**Note: Backup any sensitive information, it will be wiped completely):  <br/>
<a href="https://imgur.com/MZEaPqC"><img src="https://i.imgur.com/MZEaPqC.png" title="source: imgur.com" /></a>
<br />
<br />
Once complete, the drive will be renamed to Ventoy and will automatically open it's directory. This is where our ISOs will be stored. Go ahead and move any bootable medias you would like to contain on this device <br/>
<a href="https://imgur.com/QXRBX39"><img src="https://i.imgur.com/QXRBX39.png" title="source: imgur.com" /></a>
<br />
<br />
Now we will attempt to use the bootable disk, keep in mind that I am running this on a virtual machine so it looks a bit different. Depending on the machine, during boot you may need to press F12 to prompt the boot menu. **Make sure your UEFI/BIOS has Secure Boot disabled**  <br/>
<a href="https://imgur.com/Dm7aGrZ"><img src="https://i.imgur.com/Dm7aGrZ.png" title="source: imgur.com" /></a>
<br />
<br />
Now that we have booted into the USB, this menu should appear with a list of all bootable medias on the device. Now we can select an .ISO to test. I will be using Win10. <br/>
<a href="https://imgur.com/1qmslNL"><img src="https://i.imgur.com/1qmslNL.png" title="source: imgur.com" /></a>
<br />
<br />

It should give you option for Normal mode and Wimboot mode. If Normal mode is giving issues, Wim mode will launch a Windows image to boot. <br/>
![image](https://github.com/earvinsantiago2020/Ventoy/assets/143285871/d51d934f-ccec-4718-a228-a8e15f4f8592)

<br />
<br />

I selected Normal mode and now I am booted into Windows Setup as can be seen here.<br/>
![image](https://github.com/earvinsantiago2020/Ventoy/assets/143285871/59a00b7c-b317-4426-8bc8-ec4a6f3491b7)

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
