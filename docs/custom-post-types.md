## Custom post types

To export custom post types, you'll need to add a filter (w.g. to your themes config file) to do the following:

```php
add_filter( 'jekyll_export_post_types', function() {
	return array('post', 'page', 'you-custom-post-type');
});
```

The custom post type will be exported as a Jekyll collection. You'll need to initialize it in the resulting Jekyll site's `_config.yml`.
