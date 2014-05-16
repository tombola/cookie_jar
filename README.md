#Cookie Jar

Simple 5 minute module intended to allow differential testing for anonymous users on a drupal site.

All this module does is set a cookie in the browser according to the url, eg:

*mysite.com/cookiejar/featuretest*

sets the 'cookiejar' cookie to 'featuretest'. Whatever your custom module is, it can then simply test for that cookie and differentiate some aspect of the site for that user. 

This means that if a couple of users volunteer and are sent to a specified url, from then onwards you can test your flashy new functionality without requiring any different behaviour from the users, and without affecting the other users of the site.

**Don't forget the effect of caching!** If you are using Boost or similar, the testing user might not see flashy feature x, or they might inadvertently save flashyfeaturex into the cache for everyone to see