<h1>Wireless Traffic Cracking and Analysis</h1>

<h2>Description</h2>
Lab consist of decrypting WEP and WPA/WPA2 protected traffic and analyzing a a personally assigned WPA2 traffic file
<br />


<h2>Languages and Utilities Used</h2>

- <b>Command line</b> 
- <b>Wireshark</b>
- <b>MD5 Hash Generator</b>
- <b>Aircrack</b>
- <b>Decap</b>

<h2>Environments Used </h2>

- <b>Kali Linux VM</b>

<h2>Project walk-through:</h2>

<h3>Task A: Decrypty WEP and WPA/WP2 protected traffic</h3>

  1. Decrypt WEP traffic
<br />
<p align="center">
DNS traffic for WEP is encrypted and thus shows no results <br/>
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/7a600b37-6495-441e-b6aa-31760d5c1124"/>
<br />
<br />
Using aircrack on the lab file to find the encryption type found within<br/>
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/f958bb28-c94e-4641-94b8-3d8841471efc"/>
<br />
<br />
Crack WEP key
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/e4c32d6c-986b-412c-8d1a-e68f363651f0"/>
<br />
<br />
Use Decap on found key
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/64de63cf-3539-46ad-83da-2c395072ec00"/>
<br />
<br />
The finalized cracked WEP protocol
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/ef70eaec-168e-41f2-aeac-0fdb6cfab293"/>
<br />
<br />
  
  2. Decrypt WPA2
<br />
<p align="center">
Gather wordlist to use for aircrack
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/89af585b-ae3d-46fd-98fc-98c1f187bf7f"/>
<br />
<br />
Using the wordlist you can use it to aircrack the new cap file
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/7c5b21f3-bd77-449a-ba2d-c299d49f53a6"/>
<br />
<br />
Cracked code
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/243ca4fc-1b68-48b8-bf72-c29e048adcde"/>
<br />
<br />
After airdecap it now displays the WPA2 traffic to wireshark
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/89a65239-570a-4adc-8ef2-b7992a9b829e"/>
<br />
<br />

<h3>Task B: Decrypt specificlly assigned WPA2 traffic file</h3>
<br />
<p align="center">
Hashed my personal ID and found the corrosponding file that was created and downloaded it
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/fb942799-fb82-4a7f-ab87-c542d9a55719"/>
<br />
<br />
Moved the files onto our kali desktop
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/9425d55e-9b19-4a60-900e-0c078ab07c46"/>
<br />
<br />
Key found for P4
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/8b14274f-1757-4205-ac37-f1ca6d0c1403"/>
<br />
<br />
Decrypted P4 file
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/8b706daf-dfd8-46c8-ae2e-d2762ac8d269"/>
<br />
<br />
The final decrypted traffic of P4 displayed in wireshark
<img src="https://github.com/HimothyRobinson/CrackingAndAnalysisLab/assets/142434081/06238958-f86b-4ddf-86c2-1b23c0057fb5"/>












  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
