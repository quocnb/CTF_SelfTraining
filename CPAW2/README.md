## CPAW2 ##

The next version of `CPAW`

- Homepage : https://ctf2.cpaw.site/#!/home
- Language: English
- Key Format `Cpaw{your_key}`

### Question ###

|#|Title|Category|Score|Progress|
|--|--|--|--|--|
|1|Fragile|Web|150| |
|2|prank| Network |100|completed|
|3|HTTPS introduction| Network |100| |
|4|Illegal Packets... | Network |300| |
|5|an apartment| Crypto |100| |
|6|easy...? Turing Machine| Crypto |100| |
|7|Secret instruction| Reverse |200| |
|8|Exec me revenge| Reverse |100| |
|9B|lackboard Of Fake1| Pwn |100| |
|10|Blackboard Of Fake2| Pwn |300| |
|11|Chance| Pwn |250| |
|12|Name Editor++| Pwn |300| |
|13|Bad Container| Forensic |300| |
|14|Trace Behavior| Forensic |200| |
|15|CCpost| Stego |100| |
|16|Random Image| Stego |200| |
|17|sumsumsum| Misc |100| |
|18|BrokenBase| Misc |150| |
|19|Everyone's power| Misc |100| completed |


### Answer ###

#### prank ####
Open the pcap file, `Follow TCP` and get the zip password
to unzip `zi...p.zip` file.

In the pcap file, we can see the `flag` file has been rename to `666666` -> open `666666` file and get the flag
```
Cpaw{Washington}
```

#### Everyone's power ####
Flag is `Cpaw{DragonBall}`

J/K

Decompiler the `pyc` file with `https://github.com/wibiti/uncompyle2`. You can read the source code. From the source code, get the user and password for capture the flag.
```
Cpaw{b7089fed7f93b4916f8559599d8c3360195090d6014a6d417886339414089e49}
```
