# Desc

A program in which you can compare two strings and see whether they are the same string or not. Pretty useful, right?

# Note untuk panitia

\-

# Flow singkat solver

Intended solution adalah dengan menggunakan teknik ret2csu. [[1](https://ropemporium.com/challenge/ret2csu.html)] [[2](https://i.blackhat.com/briefings/asia/2018/asia-18-Marco-return-to-csu-a-new-method-to-bypass-the-64-bit-Linux-ASLR-wp.pdf)]

Bisa overwrite variable `str2_length` dengan value yang cukup besar (`0xff`), dengan demikian dapat tercapai buffer overflow. Karena tidak ada stack canary, exploitasi dapat dilakukan dengan mudah.
