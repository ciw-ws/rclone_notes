# rclone_notes
#### Description for this repo
*	Updated 190906
*	Requirements
*	Installation
*	Basic Usage

---

### Requirements
*	Google drive account (education account is recommended, for unlimited space)
*	Rclone installation

---

### Installation
*	Download Rclone from source (Windows, AMD64 - 64 Bit)
	*	https://rclone.org/downloads/
	*	https://downloads.rclone.org/v1.49.1/rclone-v1.49.1-windows-amd64.zip

*	Extract the downloaded zip file
*	Open a new command line window (cmd, powershell, ...)
*	Move to the root directory of rclone.exe
*	Create new rclone config, commands as below
```
.\rclone.exe config
n) New remote
gd_ncu (any name you like)
12 (google drive)
(press enter)
(press enter)
1
(press enter)
(press enter)
n
y
(login with your google drive account in the browser, allow rclone to access)
n
y
q
```

---

### Basic Usage
*	Copy
	*	.\rclone copy -v /path/to/src /path/to/dst
```
.\rclone.exe copy -v G:\rclone_examples gd_ncu:/rclone_examples
```

*	Check
	*	.\rclone check -v /path/to/src /path/to/dst
```
.\rclone.exe check -v G:\rclone_examples gd_ncu:/rclone_examples
```
