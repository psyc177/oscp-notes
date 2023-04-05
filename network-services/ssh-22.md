# SSH  22

## Login

Try logging in by using username or root user

```bash
ssh uname@10.10.10.10
```

```bash
ssh root@10.10.10.10
```

In case you don't have the normal access to ssh you can try to find the RSA key , and with the RSA key try to so ssh

```bash
ssh -i RSA.key uname@10.10.10.10
```

Just in case if your RSA is encrypted you can decrypt it first and then try to login in ssh

```
openssl rsa -in encrypt-rsa.key -out decrypt-rsa.key
ssh -i decrypt-rsa.key uname@10.10.10.10
```
