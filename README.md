# OSINT-investigations
![eye](eye.jpg)

This repository contains my OSINT investigations. The main purpose of this, is train my OSINT habilities.
{% assign subfolders = site.static_files | where_exp: "file", "file.path contains '/ruta/a/tu/directorio/'" | map: "path" | map: "split: '/'" | map: "last" | uniq %}
{% for folder in subfolders %}
- [{{ folder }}]({{ folder }}/index.md)
{% endfor %}
