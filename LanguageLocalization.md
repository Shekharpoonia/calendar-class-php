# Introduction #

Output of the calendar class can be localized to your language. Use [PHP's setlocale() function](http://www.php.net/setlocale) to output the calendar customized for your local language


## Localized Language Example ##

```
/* include the calendar class */
require_once('calendar.class.php');

/* create the calendar object */
$calendar = new Calendar('2012-12-21');

/*
 to localize the output to your language use 
 PHP's setlocale() function before you call the 
 output_calendar() method. 

 For example this will localize the calendar for German

 View PHP documentation to find the value appropriate to your location
 */
setlocale(LC_ALL, 'de_DE');

/* now output the calendar as normal */
print($calendar->output_calendar());

```


[View Working Example at Style-vs-SUBSTANCE.com](http://style-vs-substance.com/projects/calendar/examples/example_6.php)