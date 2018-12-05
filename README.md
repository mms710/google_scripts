# google_scripts
Collection of google scripts that could be useful

## pto_form_to_google_calendar Script
Note: This is basically a complete copy of the work here http://www.jessespevack.com/blog/2016/2/9/turn-a-google-form-response-into-a-calendar-event with some very minor tweaks for my own purposes.

### Summary
This script, when you put it in the script editor for a spreadsheet attached to a google form, takes the form responses from the form as they come in and turns them into calendar invites. This particular version is used to create PTO calendar entries for people when they submit PTO through the google form.

### Setup Info
1. Replace the CalendarID and formID variables at the top with your CalendarID and formID. Your calendarID can be found in the settings on your calendar you want it to post events on and your formID can be found in the URL of your google form. The URL of your google form is in the format "https://docs.google.com/forms/d/<look your form ID will be here!!!>/edit", so just copy and paste the long string of characters you find between those two slashes.
2. You'll need to add the Moments library to the Google script editor. To do that, you need to go to Resources->Libraries... in the top bar and then add the Moments library with the code "MHMchiX6c1bwSqGM1PZiW_PxhMjh3Sh48". Ensure you're on the latest version using the Versions dropdown.
3. Change the formMap entries in the global variable at the top to the names in the column headers on the spreadsheet attached to the google form.
4. When in doubt, add "Logger.log( <thing you want to log> )" or add "debugger;" to log a specific value or debug a function.
