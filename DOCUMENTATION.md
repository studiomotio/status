# Documentation
Useful documentation about how to switch to maintenance mode.

## Server

### DNS
Update domain name pointing to use **Github Pages** records:  

```dns
IN A     185.199.108.153  
IN A     185.199.109.153  
IN A     185.199.110.153  
IN A     185.199.111.153  
www      IN CNAME     studiomotio.github.io.
```

> [!NOTE]
> Be sure to remove the `IN A 54.36.182.97` record and replace the `www IN CNAME studiomotio.com.` record.

### HTTPS
Be sure to have the CNAME properly configured with `studiomotio.github.io` domain in order to **enforce HTTPS**.

> [!NOTE]
> If HTTPS does not work, removing and adding again the custom domain on Github may help.
