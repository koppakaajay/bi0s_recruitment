# Network Forensics
## Process:
Unzipped the file to get the .pcap.

Opened it with Wireshark.

Went through the packets and at the 5th Serial number there was a message stating the key was 5.

The I went through the rest of the packets and there I found a suspected string which supposedly looks like the flag and that was `gn0x{s3yb0wp_nsyjwhjuynts_l0jx_g00rc0c0}?` after using a ceaser cipher with a shift of 5 letters I found the flag.

## Flag Found 
`bi0s{n3tw0rk_interception_g0es_b00mx0x0}`

# Steganography
## Process:
### Method- 1
This can be done by using stegsolve usin the inbuilt image combiner. We need to combine the images incredible and chall. And under the SUB plane you can see the flag
### Method- 2
We can also do this by importing th numpy and PIL libraries in python
[Click here for the code](https://github.com/koppakaajay/bi0s_recruitment/blob/main/c0mb1n3d.py)

## FLAG FOUND
`flag{h4ppy_h4ppy_h4ppy_:)}`  

# Image Forensics
## PNG
### c0rrupt3d
#### Process:
Just fixed Magic numbers for the png image as 89 50 4E 47 0D 0A 1A 0A and got the flag.
#### FLAG FOUND:
`vidyutctf{4r3_y4_w1nn1ng_s0n}`

### 3nc1m4g3
#### Process:
wrote a python script which xors the magic numbers of the png with actual magic numbers of a png to obtain the key. The it xors the whole image with key. The result here was a QR code. So I used another script to get the text out of the QR code.
#### FLAG FOUND:
`flag{x0r_1s_c00l;)}`

