# WP_ObjVarDump
WordPress var_dump safe hook to extract object data, get_current_screen

#NOTE: ``` get_current_screen() ``` is checking which type of object you are currently working with ex. what post_type etc... 

```PHP
 // Admin Hook: https://developer.wordpress.org/reference/hooks/admin_notices/
 add_action('admin_notices', function() {
  
   $screen = get_current_screen();
   var_dump($screen);  

 });

 // Public Hook
 add_action('init', function() {

   $posts = Get_Object;
   var_dump($posts);  

 });

```
<br />Also: 
<br /> https://developer.wordpress.org/reference/hooks/all_admin_notices/
