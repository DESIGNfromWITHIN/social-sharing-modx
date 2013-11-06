# Social Sharing MODX
Add social sharing links and buttons without the bloat for MODX Revolution (based on [Social Sharing](https://github.com/cferdinandi/social-sharing)).

The widgets provided by Twitter, Facebook, and other services require numerous HTTP requests and can really hurt the performance of your sites and apps. These simple CSS and HTML snippets make it easy for you to go social - without hurting site performance.

## How It Works
<h3>MODX tag that are used</h3>
<ul>
    <li>&#91;&#91;*longtitle:empty=`&#91;&#91;*pagetitle&#93;&#93;`&#93;&#93; - The longtitle of the page (if it is empty the pagetitle is used)</li>
    <li>&#91;&#91;!++site_url&#93;&#93;&#91;&#91;*uri&#93;&#93; - The URL of page</li>
    <li>&#91;&#91;*description&#93;&#93; - The page description</li>
    <li>&#91;&#91;*description&#93;&#93; - The page description</li>
</ul>

<h3>Extra Template Variables that are used (these need to be created)</h3>
<ul>
    <li>&#91;&#91;*social-sharing-modx_twitter_id&#93;&#93; - Needed for the Twitter ID</li>
    <li>&#91;&#91;*social-sharing-modx_pinterest_img&#93;&#93; - Needed for the Pinterest thumbnail</li>
</ul>

<h2>The MODX tags</h2>

<p><strong>Twitter</strong><br>
&lt;a target="_blank" href="https://twitter.com/intent/tweet?text=[[*longtitle:empty=`[[*pagetitle]]`]]&url=[[!++site_url]][[*uri]]&via=[[*social-sharing-modx_twitter_id]]">Twitter&lt;/a></p>
<p><strong>Facebook</strong><br>
&lt;a target="_blank" href="http://www.facebook.com/sharer/sharer.php?u=[[!++site_url]][[*uri]]">Facebook&lt;/a></p>
<p><strong>Google+</strong><br>
&lt;a target="_blank" href="https://plus.google.com/share?url=[[!++site_url]][[*uri]]">Google+&lt;/a></p>
<p><strong>LinkedIn</strong><br>
&lt;a target="_blank" href="http://www.linkedin.com/shareArticle?mini=true&url=[[!++site_url]][[*uri]]&title=[[*longtitle:empty=`[[*pagetitle]]`]]&summary=[[*description]]&source=[[!++site_url]][[*uri]]">LinkedIn&lt;/a></p>
<p><strong>Pinterest</strong><br>
&lt;a target="_blank" href="http://pinterest.com/pin/create/button/?url=[[!++site_url]][[*uri]]&description=[[*description]]&media=[[++site_url]][[*social-sharing-modx_pinterest_img]]">Pinterest&lt;/a></p>

## Changelog
* Version 1.0 (november 6, 2013)
  * Initial release.

## License
Social Sharing MODX is free to use under the [MIT License](http://gomakethings.com/mit/).

## Thanks
Social Sharing MODX is based on [Social Sharing](https://github.com/cferdinandi/social-sharing) from [Chris Ferdinandi](https://github.com/cferdinandi).
Forked and updated for MODX Revolution by [Menno Pietersen](https://github.com/DESIGNfromWITHIN) from [Any Screen Size](http://anyscreensize.com)