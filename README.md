Marketo Canadian Opt-in
========================

If the user has or selects a country from a dropdown where an opt-in rather than an opt-out is required, uncheck the opt-in checkbox.

Install
========================

Load the canadianoptin.js file into the design studio.

Update the path to the canadianoptin.js file in the code below.

Update the field name for the country select in the countryfield variable. (Be sure to use the name and not the ID)

Update the field name for the opt-in checkbox in the optinfield variable.  (Be sure to use the name and not the ID)

Update the list of disallowed values from the country select.  (This is an array)

```HTML
<script type="text/javascript">
var countryfield = "Country";
var optinfield = "marketingOptIn";
var disallowedprepop = ["Canada", "CA", "CAN"]
</script>
<script src='//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js' ></script>
<script src='** PATH TO THE canadianoptin.js FILE' ></script>
```

Place the code above, after you have updated it, into the page code below the code to create the form.  The bottom of the page, right above the closing </body> tag works fine.