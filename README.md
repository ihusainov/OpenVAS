# OpenVAS


 **Update library**
```bash
greenbone-feed-sync --type GVMD_DATA
greenbone-feed-sync --type SCAP
greenbone-feed-sync --type CERT
greenbone-nvt-sync
greenbone-certdata-sync
greenbone-scapdata-sync
```

#Upgrade from 20.08 to 21.04

```bash
Stop all services (gvmd, gsad, ospd-openvas…)
Configure, build and install all 21.04 modules, starting with gvm-libs like you did for 20.08
Migrate your database with “gvmd -m” command
Start gvmd, ospd-openvas then gsad like you did before
```


**After upgrade need start**
```bash
gvmd --rebuild
```

**Modules**
```bash
GVM Libraries 21.4.1 100
openvas scanner 21.4.1 88
ospd 21.4.1 15
ospd-openvas 21.4.1 12
Greenbone Vulnerability Manager 21.4.2 41
Greenbone Security Assistant 21.4.1 24
```
