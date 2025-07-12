# picoCTF: DISKO 1

**Category:** Forensics  
**Points:** 100  
**Difficulty:** Easy  
**Platform:** picoCTF 2025

---

## Challenge Description

> Can you find the flag in this disk image?  
> [Download the disk image](https://artifacts.picoctf.net/c/538/disko-1.dd.gz)

---

## Tools Used

- Git Bash
- `gunzip`
- `grep -a`

---

## Solution Summary

1. Downloaded `.dd.gz` and extracted using `gunzip`.
2. Used `grep -a "picoCTF{" disko-1.dd` to search the raw disk.
3. Found the flag as plain text.

---

## Screenshots

![Step 1](./img/step1_downloaded.png)  
![Step 2](./img/step2_downloaded.png)  
![Step 3](./img/step3_downloaded.png)

