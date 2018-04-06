# CPAW #

## LEVEL 2 ##

- [x] [Stego]隠されたフラグ
- [x] [Web] Redirect
- [x] [Network+Forensic]HTTP Traffic
- [ ] [Recon]Who am I ?
- [x] [Forensic]leaf in forest
- [x] [Misc]Image!
- [x] [Crypto]Block Cipher
- [ ] [Reversing]reversing easy!
- [ ] [Web]Baby's SQLi - Stage 1
- [x] [Network] Can you login？

### [Stego]隠されたフラグ ###
You can see the `morse code` in the top-left and bottom-right of the image.

flag is `cpaw{hidden_message:)}`

### [Web] Redirect ###
Check url header info
```
curl -D -  http://q15.ctf.cpaw.site
```
Flag
```
cpaw{4re_y0u_1ook1ng_http_h3ader?}
```

### [Network+Forensic]HTTP Traffic ###
Open `pcap` file by Wireshark. Then export all http resource by
```
File > Export Object > HTTP
```

Open the `network100` the source code, change the `image.jpg` and `button2.js` file to right place.

Just run `network100` by web-browser and see the flag
```
cpaw{Y0u_r3st0r3d_7his_p4ge}
```

### [Forensic]leaf in forest ###
Open file by `Atom`, remove all `lovelive!` text, you will get
```
CCCelivelovelivPPPovelive!loveAAAe!lovWWWve!{{{elive!loveliMMMelive!lovelGGG!lovelivRRRovelive!lEEElive!PPPelive!}}}
```
Keep remove all unnecessary text you will get
```
CCCPPPAAAWWW{{{MMMGGGRRREEEPPP}}}
```
Flag is
```
cpaw{mgrep}
```

### [Misc]Image! ###
Check file type
```
file misc100.zip
// misc100.zip: OpenDocument Drawing
```
Open it by OpenDocument software and see the Flag

### [Crypto]Block Cipher ###
Just run the `crypto100.c` with parameter
`ruoYced_ehpigniriks_i_llrg_stae` and the key (number)

Flag
```
cpaw{Your_deciphering_skill_is_great}
```

### [Network] Can you login？ ###
Open `pcap` file by `Wireshark` you can get some information

```
HOST 157.7.52.186:21
USER cpaw_user
PASS 5f4dcc3b5aa765d61d8327deb882cf99
```

FTP to the HOST and get the `flag` in `.hidden_flag_file`

Flag
```
cpaw{f4p_sh0u1d_b3_us3d_in_3ncryp4i0n}
```
