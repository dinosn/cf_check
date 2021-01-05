# cf_check
cloudflare ip check and exclude.

Given a file with IP addresses parse them fast to exclude IP addresses related to cloudflare. 

```grep -vf cloudflare_check.txt ip_file.txt```

Original cloudflare ip addresses can be found at https://www.cloudflare.com/ips/, expanding them directly will create 1.786.880 distinct ip records which will consume significant memory on grep and will get it killed. 
