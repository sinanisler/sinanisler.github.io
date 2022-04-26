## WordPress Developer Library
Usefull Snippets, Functions and Codes for developing WordPress Themes.



```php

<ul class="cat-list">
  <?php wp_list_categories( array(
      'orderby'    => 'name',
      'show_count' => false,
      'title_li' => '',
      'hierarchical'=> true
  ) ); 

  $all_categories=get_categories();
  foreach($all_categories as $categories_item)
  {
    echo "<li>".$categories_item->description."</li>";
  }

  ?> 
</ul>


```
