# Crackmes Chalenges

Solved by KryptoPX

| Name               | User   | Link                                                  | Branch      | Lang |
| ------------------ | ------ | ----------------------------------------------------- | ----------- | ---- |
| SimpleButDangerous | EaminX | https://crackmes.one/crackme/62e518b533c5d44a934e9a4c | challenge-0 | .NET |

---

## Tools used

- Detect It Esay
  - Confuser(1.X)[-]
  - Dotfuscator(-)[-]
  - Eazfuscator(-)[-]
  - Goliath(-)[-]
  - Babel .NET(3.X)[-]
  - Yano(1.X)[-]
- De4dotFixAntide4dot
  - Run 3 times
- DNSpy
- CyberCheff
  
## Steps

1. Detect obfuscator using detect it esay
    - 6 obfuscators detected
2. Go to Form1, second if (Token: 0x0100006B)

```C#
@string = Encoding.UTF8.GetString(Convert.FromBase64String("YzNWd1pYSnpaWGg1"));
```

3. using CyberCheff decode two times using FromBase64

```C#
YzNWd1pYSnpaWGg1 => c3VwZXJzZXh5 => supersexy
```

## password is supersexy


