#Migración SQL
Migración de dominio via SQL tradicional

##Options wp_options
```UPDATE `wp_options` SET `option_value` = REPLACE(`option_value`, 'https://easyrentals.es/', 'https://erreproperties.com') WHERE `option_value` LIKE '%https://easyrentals.es/%' COLLATE utf8mb4_bin```


