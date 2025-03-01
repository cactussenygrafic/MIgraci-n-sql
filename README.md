<h1>Migración SQL</h1>
Migración de dominio via SQL tradicional

<h2>Options (wp_options)</h2>
<code>UPDATE `wp_options` SET `option_value` = REPLACE(`option_value`, 'https://easyrentals.es/', 'https://erreproperties.com') WHERE `option_value` LIKE '%https://easyrentals.es/%' COLLATE utf8mb4_bin</code>
<br><br>
<h2>Posts (wp_posts)</h2>
<code>UPDATE `wp_posts` SET `post_content` = REPLACE(`post_content`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `post_content` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_posts` SET `guid` = REPLACE(`guid`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `guid` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<h2>YOAST</h2>
<code>UPDATE `wp_yoast_seo_links` SET `url` = REPLACE(`url`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `url` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_yoast_indexable` SET `permalink` = REPLACE(`permalink`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `permalink` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_yoast_indexable` SET `twitter_image` = REPLACE(`twitter_image`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `twitter_image` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_yoast_indexable` SET `open_graph_image` = REPLACE(`open_graph_image`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `open_graph_image` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_yoast_indexable` SET `open_graph_image_meta` = REPLACE(`open_graph_image_meta`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `open_graph_image_meta` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>

<br><br>
<h2>Post meta</h2>
<code>UPDATE `wp_postmeta` SET `meta_value` = REPLACE(`meta_value`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `meta_value` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>

<br><br>
<h2>Users</h2>
<code>UPDATE `wp_users` SET `user_url` = REPLACE(`user_url`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `user_url` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_usermeta` SET `meta_value` = REPLACE(`meta_value`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `meta_value` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>

<br><br>
<h2>WPML</h2>

<code>UPDATE `wp_icl_translation_status` SET `translation_package` = REPLACE(`translation_package`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `translation_package` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_icl_translation_status` SET `_prevstate` = REPLACE(`_prevstate`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `_prevstate` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_icl_string_translations` SET `value` = REPLACE(`value`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `value` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
<br><br>
<code>UPDATE `wp_icl_strings` SET `value` = REPLACE(`value`, 'https://easyrentals.es', 'https://erreproperties.com') WHERE `value` LIKE '%https://easyrentals.es%' COLLATE utf8mb4_bin</code>
