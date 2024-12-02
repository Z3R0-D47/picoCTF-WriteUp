# Description
People keep trying to trick my players with imitation flags. I want to make sure they get the real thing! I'm going to provide the SHA-256 hash and a decrypt script to help you know that my flags are legitimate.
```bash
ssh -p 59025 ctf-player@rhea.picoctf.net
```

* Using the password:
  
```bash
84b12bae
```
* Accept the fingerprint with `yes`, and `ls` once connected to begin. Remember, in a shell, passwords are hidden!

* Checksum: `3ad37ed6c5ab81d31e4c94ae611e0adf2e9e3e6bee55804ebc7f386283e366a4`

To decrypt the file once you've verified the hash, run: 
```bash
./decrypt.sh files/<file>.
```

## Step-by-Step Solution
After connected using ssh
### 1. Listing Files 
List the files in the directory using `ls` command.

Output Shown:
```bash
checksum.txt  decrypt.sh  files
```

### 2. Checking the Provided Checksum
Next, we look at the contents of checksum.txt by using `cat` command, which contains the target SHA256 hash:

```bash
cat checksum.txt
```
Output Shown Following Hash:
```bash
3ad37ed6c5ab81d31e4c94ae611e0adf2e9e3e6bee55804ebc7f386283e366a4
```

### 3. Generating SHA256 Hashes for Files

