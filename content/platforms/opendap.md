---
section: Platforms
nav_order: 19
title: Opendap
---

You can access directly the extraction files via [MEOM Opendap](https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/catalog/meomopendap/extract/MEOM/catalog.html)

You can navigate through the directories and download a file by clicking on its name and on the HTTPServer link or you can get a given file via wget command : ```wget https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/MEOM/eNATL60/eNATL60-BLBT02/1h/SICIL/eNATL60SICIL-BLBT02_y2010m09d30.1h_vozocrtx.nc```

If you need to download multiple files, consider the following compact command :
```bash
wget https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/MEOM/eNATL60/eNATL60-BLBT02/1h/SICIL/eNATL60SICIL-BLBT02_y20{09..10}m{01..12}d{01..31}.1h_vozocrtx.nc
```
or a script of the form :

```bash
for var in vozocrtx votemper vosaline vomecrty; do
  wget https://ige-meom-opendap.univ-grenoble-alpes.fr/thredds/fileServer/meomopendap/extract/MEOM/eNATL60/eNATL60-BLBT02/1h/SICIL/eNATL60SICIL-BLBT02_y20{09..10}m{01..12}d{01..31}.1h_${var}.nc
done
```

All the extractions already hosted on opendap are listed below :

{% include list_extract_opendap.html %}


And you can also find some configuration files :

{% include list_config_opendap.html %}


