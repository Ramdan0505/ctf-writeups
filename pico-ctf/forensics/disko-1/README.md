

# picoCTF: DISKO 1

**Category:** Forensics  
**Points:** 100  
**Difficulty:** Easy  
**Platform:** picoCTF 2025

---

## Challenge Description

> Can you find the flag in this disk image?  
> Download the disk image [here](https://artifacts.picoctf.net/c/538/disko-1.dd.gz)

---

## Tools Used

- Git Bash (Windows)
- `gunzip` – decompress `.gz` file
- `grep -a` – scan binary files for embedded text

---

## Step-by-Step Solution

### Step 1: Create a working folder

```bash
mkdir -p ~/pico_disko1
cd ~/pico_disko1

Step 2: Download and extract the disk image
bash
Copy code
curl -L -o disko-1.dd.gz "https://artifacts.picoctf.net/c/538/disko-1.dd.gz"
gunzip disko-1.dd.gz
You should now have a 50MB file named disko-1.dd.

Step 3: Search for the flag string inside the image
bash
Copy code
grep -a "picoCTF{" disko-1.dd
The -a flag tells grep to treat the binary .dd file as text.

Since the flag is embedded in plaintext, this reveals it instantly.

Step 4: Copy and submit the flag
Once the string appears, copy the full picoCTF{...} and submit it on picoCTF.

## Solution Summary

1. Downloaded `.dd.gz` and extracted using `gunzip`.
2. Used `grep -a "picoCTF{" disko-1.dd` to search the raw disk.
3. Found the flag as plain text.
4. copy and submit flag



Challenge complete!

---

## Screenshots

![Step 1](./img/step1_downloaded.png)  
![Step 2](./img/step2_downloaded.png)  
![Step 3](./img/step3_downloaded.png)

