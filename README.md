# henry-schein-take-home-test

Because this app is so small, I didn't bother to creat MVC directories.
I didn't use String.split(), because my auto-fill says it takes a regex, which is off-limits for this assignment.
There are no doubt other ways to accomplish this task, but without using regex, this was the most efficient way I came up with in my short time working tonight.

Use postman to post this body to http://localHost:8080/parse
  "Patient Name","SSN","Age","Phone Number","Status"
  "Prescott, Zeke","542-51-6641",21,"801-555-2134","Opratory=2,PCP=1"
  "Goldstein, Bucky","635-45-1254",42,"435-555-1541","Opratory=1,PCP=1"
  "Vox, Bono","414-45-1475",51,"801-555-2100","Opratory=3,PCP=2"

Thanks!
