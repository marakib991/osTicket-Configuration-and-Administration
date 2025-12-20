# osTicket-Configuration-and-Administration

## Overview

This project simulates the practical steps involved in setting up and managing an osTicket helpdesk system. It covers environment preparation, installation, configuration of roles, departments, SLAs, and help topics, as well as demonstrating key skills in IT support workflows and ticket management.

## Environment Setup

### Install and configure XAMPP and osTicket zip

#### Download XAMPP v8.1.25:

Downloaded XAMPP v8.1.25 because osTicket doesn't support any version newer or older than v8.1.

<img width="1624" height="715" alt="Image" src="https://github.com/user-attachments/assets/b1128f24-f5a7-4223-b07b-bd97472b792c" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/eacafd08-f2e6-4787-9957-6b59d73017b3" />
<img width="1624" height="408" alt="Image" src="https://github.com/user-attachments/assets/195dd2a7-ac03-4d52-9fe4-49cdd5bb0653" />

---

#### Download osTicket v1.18.2:

Download the **osTicket** zip file from the official _GitHub_ page.

<img width="1624" height="692" alt="Image" src="https://github.com/user-attachments/assets/30ce8090-afb2-4db1-bb65-71c0f6f879ce" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/e0c02942-e537-49a8-9141-511400b640f7" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/9f0f1065-7910-4dc3-bcf6-6d1472336b5a" />
<img width="1624" height="640" alt="Image" src="https://github.com/user-attachments/assets/89732316-25ff-45fa-968b-f9c5bf0bb1af" />

---

#### Install XAMPP:

Navigate to the download folder and install the **XAMPP** to `C:\XAMPP` so it doesn't interfere with the user security policy.

<img width="1624" height="862" alt="Image" src="https://github.com/user-attachments/assets/59622a5d-31a0-4dde-8510-a7bf22fa47e0" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/9cd9d769-b04a-4d3f-a979-87f0e8f26170" />

---

#### Extract osTicket zip:
Extracted the zip file to `c:\XAMPP\htdocs`. Created a new folder _osTicket_ and extracted the zip there.

<img width="1624" height="825" alt="Image" src="https://github.com/user-attachments/assets/b2ef7693-870e-4ffa-ac2c-584fb4878a30" />
<img width="1624" height="801" alt="Image" src="https://github.com/user-attachments/assets/b8d8ecf2-aa9b-45f6-8503-1c1ffb571d10" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/8306ee33-60ee-404e-9c97-307aa1e55793" />
<img width="1624" height="858" alt="Image" src="https://github.com/user-attachments/assets/7628564e-0302-47f2-baad-fb5b694f924b" />
<img width="1624" height="1005" alt="Image" src="https://github.com/user-attachments/assets/4b72d758-5ad8-4707-bd74-7fd1ed0ee65c" />
<img width="1624" height="839" alt="Image" src="https://github.com/user-attachments/assets/5a781e90-2461-41f7-b988-686166f80521" />
<img width="1624" height="879" alt="Image" src="https://github.com/user-attachments/assets/e6156617-830c-4aaf-bc96-0e385c27b8db" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/ac0dbfff-6d02-449c-91fd-e89c7a541239" />

---

#### _ost-sampleconfig.php_ configuration:

Navigate to _ost-sampleconfig.php_ file and renamed it and check if the writable permission is granted.

<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/0b1e221a-5dfa-423e-9019-cf11844b8cf3" />
<img width="1624" height="883" alt="Image" src="https://github.com/user-attachments/assets/884b9ce3-eb48-46f3-8d5f-7f18177e1bb1" />
<img width="1624" height="880" alt="Image" src="https://github.com/user-attachments/assets/504bf16b-cf74-4d0c-b420-af74afc329d5" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/3fe313c0-f2ad-4ced-a329-c5df4db387ec" />

---

## Install and Configure osTicket
### Installation Steps

#### Created Database: In phpMyAdmin, create a database named **osticket**:
Run **XAMPP** and start **Apache** and **MySQL**. Then went to **phpMyAdmin** and created the **osticket** database.

<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/a35898a2-f448-4d08-987e-36d529fd8fcb" />
<img width="1624" height="656" alt="Image" src="https://github.com/user-attachments/assets/66d009dc-db85-4f32-9113-a4881e8d0b2f" />
<img width="1624" height="662" alt="Image" src="https://github.com/user-attachments/assets/bc8bf7b7-70ae-4898-9913-4be7e27349a9" />
<img width="1037" height="530" alt="Image" src="https://github.com/user-attachments/assets/9c23fdc8-365f-43be-bfcb-b4871d7cf9ed" />
<img width="1624" height="556" alt="Image" src="https://github.com/user-attachments/assets/9acb7d9e-ac1e-46c9-a1d8-f709782a8c51" />
<img width="1624" height="650" alt="Image" src="https://github.com/user-attachments/assets/29466eab-7feb-4f84-abf6-38fe91621725" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/5359aec6-50c4-4be9-a0ed-2ab1bff81309" />
<img width="1398" height="493" alt="Image" src="https://github.com/user-attachments/assets/754d6695-2579-402b-8e41-c11f7b2596cb" />
<img width="1624" height="623" alt="Image" src="https://github.com/user-attachments/assets/d75f3ae7-b73e-4811-bc80-e27e6ee01b29" />
<img width="1624" height="994" alt="Image" src="https://github.com/user-attachments/assets/1b0d9083-22df-48bb-ab7c-e4554acc6d44" />

---

#### Set a password for the **root** user in **phpMyAdmin**:
Set a password which will be required during the osTicket installation. After creating the password, navigate to _config.inc.php_ file and put the newly created password in the empty field of the **server's password** section. Now, **phpMyAdmin** will be able to log the user in with new credentials.

<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/dc3bb317-1e16-47bc-a07c-2a55aacf5d87" />
<img width="1622" height="660" alt="Image" src="https://github.com/user-attachments/assets/267955f5-4372-41a4-b044-8bf5527cf459" />
<img width="1622" height="795" alt="Image" src="https://github.com/user-attachments/assets/8eda40f6-c2b0-4e9b-8d48-9d92640d3688" />
<img width="1622" height="515" alt="Image" src="https://github.com/user-attachments/assets/2a71a6fd-b6dd-4c6f-96bc-d04b14e358da" />
<img width="1619" height="900" alt="Image" src="https://github.com/user-attachments/assets/91f693ac-2d38-49c6-bad4-2b89c503bd79" />
<img width="1204" height="695" alt="Image" src="https://github.com/user-attachments/assets/ee377c3c-651e-423e-803e-482ece44eb94" />
<img width="1259" height="344" alt="Image" src="https://github.com/user-attachments/assets/3d370643-ce9f-4f6e-8dec-0f872c5c7781" />
<img width="1428" height="675" alt="Image" src="https://github.com/user-attachments/assets/fb12416f-5cf8-4f30-a317-76b90cb60df1" />

---



#### Installed osTicket:
Installed osTicket from localhost by filling the form with accurate credentials.

<img width="1451" height="523" alt="Image" src="https://github.com/user-attachments/assets/36388ce2-52c8-4d34-a2ec-f00ce21268fd" />
<img width="1215" height="484" alt="Image" src="https://github.com/user-attachments/assets/83fda572-d38a-41cb-aa7e-a8707e5e96f0" />
<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/1e41bb1e-6939-4caf-bf6b-5ab98980e570" />
<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/930e9eeb-8e40-4198-b6fb-01823a73a5e7" />
<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/dbca803b-6e3a-4cb4-81aa-d046857aecea" />
<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/2ecb638a-7018-4cec-95f3-55bff9a18b0b" />
<img width="1622" height="996" alt="Image" src="https://github.com/user-attachments/assets/2344b055-6a4f-4414-97d5-e4188c69c9ba" />

---



