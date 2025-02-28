#Migración SQL
Migración de dominio via SQL tradicional

<h2>Options wp_options</h2>
<code>UPDATE `wp_options` SET `option_value` = REPLACE(`option_value`, 'https://easyrentals.es/', 'https://erreproperties.com') WHERE `option_value` LIKE '%https://easyrentals.es/%' COLLATE utf8mb4_bin
</code>

<h2>wp_posts</h2>
<code>UPDATE `w47fa_posts` SET `post_content` = REPLACE(`post_content`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `post_content` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<hr/>
<code>UPDATE `w47fa_posts` SET `guid` = REPLACE(`guid`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `guid` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>

<h2>wp_yoast_seo_links</h2>
<code>UPDATE `w47fa_yoast_seo_links` SET `url` = REPLACE(`url`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `url` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>

