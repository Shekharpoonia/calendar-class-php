# Introduction #

Flexible formating of the URL that dates link to is now possible thru the property, $formatted\_link\_to(). Simply provide a string containing [PHP date() function](http://www.php.net/manual/en/function.date.php) compatible parameters. Not only does this new feature allow better control of the URL that days link to, it also allows calendar.class.php to integrate into applications utilizing Cruft-free URLs.



## Formatted Link Example ##

```
/* include the calendar class */
require_once('calendar.class.php');

/* create the calendar object */
$calendar = new Calendar('2012-12-21');

/*
 provide a date() function friendly formatting string for the day links

 The formatting string below produces a link like this
 http://yourdomain.com/2012/12/21
*/
$calendar->formatted_link_to = '/%Y/%m/%d';

/* now output the calendar as normal */
echo $calendar->output_calendar();
```


[View Working Example at Style-vs-SUBSTANCE.com](http://style-vs-substance.com/projects/calendar/examples/example_25_2.php)