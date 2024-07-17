---
short_name: jill
name: Jill Smith
position: Chief Editor
tags: ['foo', 'bar', 'baz']
title: "Jill Smith 的页面"
---
Jill is an avid fruit grower based in the south of France.

[Link to a post]({% link _posts/2018-08-20-bananas.md %})

{{ page.path }}

{% post_url 2018-08-20-bananas %}

[Name of Link]({% post_url 2018-08-20-bananas %})

{{ "hi" | capitalize }}

{{ "/assets/style.css" | absolute_url }}

{{ site.time | date_to_xmlschema }}

{{ site.time | date_to_rfc822 }}

{{ site.time | date_to_string }}

{{ site.time | date_to_string: "ordinal", "US" }}

{{ site.time | date_to_long_string }}

{{ site.time | date_to_long_string: "ordinal" }}

{{ "foo, bar; baz?" | cgi_escape }}

{{ "http://foo.com/?q=foo, \bar?" | uri_escape }}

{{ "Hello world!" | number_of_words }}

{{ "你好hello世界world" | number_of_words }}

{{ "你好hello世界world" | number_of_words: "cjk" }}

{{ "你好hello世界world" | number_of_words: "auto" }}

{{ page.tags | array_to_sentence_string }}

{{ page.excerpt | markdownify }}

{{ page.title | smartify }}

{{ "The _config.yml file" | slugify }}

{{ "The _config.yml file" | slugify: "pretty" }}

{{ "The _cönfig.yml file" | slugify: "ascii" }}

{{ "The cönfig.yml file" | slugify: "latin" }}

{{ site.data.navigation | jsonify }}

{{ "a \n    b" | normalize_whitespace }}

{{ page.tags | sort }}


{{ page.tags | push: "Spokane" }}

{{ page.tags | pop }}

{{ page.tags | shift }}

{{ page.tags | unshift: "Olympia" }}

{{ page.tags | inspect }}