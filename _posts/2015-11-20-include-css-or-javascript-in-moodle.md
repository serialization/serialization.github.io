---
title: "Include CSS or JavaScript in Moodle"
categories: [Moodle]
---

To include a CSS file in Moodle:

{% highlight php %}
<?php
  $PAGE->requires->css(new moodle_url('/path/to/file.css'));
?>
{% endhighlight %}

To include a JavaScript file in Moodle:

{% highlight php %}
<?php
  $PAGE->requires->js(new moodle_url('/path/to/file.js'));
?>
{% endhighlight %}

Provide the relative path to the file (excluding document root).

When writing a custom plugin, place CSS in a file called `styles.css` in the base directory of your plugin `/plugin/styles.css`. Moodle will automatically load the CSS file for you.