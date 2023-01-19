# Openclash Comic Rules List

A rules that contains comic site list based on tachiyomi extension.

How to use :

1. Add the .yaml file to openclash rule_provider folder.
2. Copy this to your config on "rule-providers" line.
```
rule_komik:
  type: file
  behavior: classical
  path: "./rule_provider/rule_komik.yaml"
 ```
 3. Copy this to your config "rules" line
 ```
 - RULE-SET,rule_komik,Komik
 ```
 4. Then you should make a new proxy grup on your config.
 
 example :
 ```
 - name: Komik
  type: select
  proxies:
  - REJECT
  - Route ID
  - Route SG
  - Route BACKUP
  use:
  - BACKUP-SERVER
  ```
  proxies name are flexible to change based on your current config
  
  5. Enjoy the joy!
