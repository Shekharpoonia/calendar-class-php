Download calendar.class.php and included it into your PHP script. Then call the constructor to create a new calendar object. Use the output method to display the calendar.

In this simplest of use (calling the constructor without any additional parameters) the class will display a calendar of the current month with today's date indicated with the css class 'today' so that it can be styled.


## Simple Use Example ##

```
/* include the calendar class */
require_once('calendar.class.php');

/* create the calendar object */
$simple_example = new Calendar();

/* now output the calendar */
echo $simple_example->output_calendar();
```

[View Working Example at Style-vs-SUBSTANCE.com](http://style-vs-substance.com/projects/calendar/examples/example_1.php)


## Displaying a Specific Month ##

To display a calendar of a specified month, you must pass two parameters to the constructor, $year and $month

```
/* include the calendar class */
require_once('calendar.class.php');

/* create the calendar object */
$simple_example = new Calendar('2012', '12');

/* now output the calendar */
echo $simple_example->output_calendar();
```


## Displaying a Calendar for a Specific Date ##

Provide a full date in YYYY-MM-DD format and calendar.class.php will output the correct month with the specified date marked with the css class 'selected' ready for you to style.

```
/* include the calendar class */
require_once('calendar.class.php');

/* create the calendar object */
$simple_example = new Calendar('2012-12-21');

/* now output the calendar */
echo $simple_example->output_calendar();
```