# AirKeyboard 1.9.0.0 Integer Overflow to Remote Denial of Service (DoS)



<br>

**AirKeyboard 1.9.0.0 suffers from an integer overflow vulnerability in its TCP request handler. The ReadLength method parses a 4-byte user-supplied length field without bounds checking, allowing attackers to trigger a denial-of-service by sending a malformed packet with an oversized length value. Exploitation requires no authentication and affects the default TCP port (55535).**

<br>

running the exploit <br>
```bash
python exploit.py
```

![image](https://github.com/user-attachments/assets/3ec10c4c-7ff0-42ab-8872-07e1f00b8412)

<br> 
on windows

![image](https://github.com/user-attachments/assets/d30f466b-8bf2-47fe-802d-bd27c0123572)
