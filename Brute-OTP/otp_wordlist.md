```
seq 0 9999 | awk '{printf "%04d\n", $1}' > otp.txt
```