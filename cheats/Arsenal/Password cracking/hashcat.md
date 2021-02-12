# hashcat

% password recovery, password cracking

#plateform/linux  #target/local  #cat/CRACKING/PASSWORD 

## hashcat - basic md5 (joomla/wordpress) - wordlist
```
hashcat -a 0 -m 400 hashes <wordlist>
```

## hashcat - basic md5 (joomla/wordpress) - wordlist with rules
```
hashcat -a 0 -m 400 hashes <wordlist> -r /usr/share/doc/hashcat/rules/best64.rule 
```

## hashcat - kerberos ticket
```
hashcat -m 18200 --force -a 0 hashes <wordlist> 
```

## hashcat - LM
```
hashcat -m 3000 -a 0 hashes <wordlist> 
```

## hashcat - NTLM
```
hashcat -m 1000 -a 0 hashes <wordlist> 
```

## hashcat - NTLMv1
```
hashcat -m 5500 -a 0 hashes <wordlist> 
```

## hashcat - NTLMv2
```
hashcat -m 5600 -a 0 hashes <wordlist> 
```

= wordlist: /usr/share/wordlist/rockyou.lst