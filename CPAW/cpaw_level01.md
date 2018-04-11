# CPAW #

## LEVEL 1 ##
| Point | Question | Answer | Done Percent
| -- | -- | -- | -- |
| 10 | 9 | 9 | 100% |

- [x] [Misc] Test Problem
- [x] [Crypto] Classical Cipher
- [x] [Reversing] Can you execute
- [x] [Misc] Can you open this file ?
- [x] [Web] HTML Page
- [x] [Forensics] River
- [x] [Network]pcap
- [x] [Crypto]HashHashHash!
- [x] [PPC]並べ替えろ!

### [Reversing] Can you execute ###
Simple using `Terminal` to get the flag
```
chmod 777 exec_me
./exec_me
```
The flag is
```
cpaw{Do_you_know_ELF_file?}
```

### [Misc] Can you open this file ? ###
```
cpaw{Th1s_f1le_c0uld_be_0p3n3d}
```

### [Web] HTML Page
```
cpaw{9216ddf84851f15a46662eb04759d2bebacac666}
```

### [Forensics] River ###
See the `location` info of the image. From location, get the name of river
```
cpaw{koutsukigawa}
```

### [Network]pcap ###
Simple open file by `Text Editor` and search the flag
```
cpaw{gochi_usa_kami}
```

### [Crypto]HashHashHash! ###
Using the hash decoder in the internet
```
cpaw{Shal}
```

### [PPC]並べ替えろ! ###
Simple sort the array and get result
```
cpaw{2112102072011931901881711671601591511501461441431361301211191111101091081051031021009994938785828180777672666360585755545250494642413634333127252420191815141210743210}
```
