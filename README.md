# henry-schein-take-home-test

Assignment:

                Using best practices complete the following task:
                Create a restful web service that takes a string of CSV data as input and returns the data reformatted as
                shown below without using regular expressions or a 3 rd party CSV parser library.
                Example input string:
                &quot;Patient Name&quot;,&quot;SSN&quot;,&quot;Age&quot;,&quot;Phone Number&quot;,&quot;Status&quot;
                &quot;Prescott, Zeke&quot;,&quot;542-51-6641&quot;,21,&quot;801-555-2134&quot;,&quot;Opratory=2,PCP=1&quot;
                &quot;Goldstein, Bucky&quot;,&quot;635-45-1254&quot;,42,&quot;435-555-1541&quot;,&quot;Opratory=1,PCP=1&quot;
                &quot;Vox, Bono&quot;,&quot;414-45-1475&quot;,51,&quot;801-555-2100&quot;,&quot;Opratory=3,PCP=2&quot;
                Return string for the above sample input
                [Patient Name] [SSN] [Age] [Phone Number] [Status]
                [Prescott, Zeke] [542-51-6641] [21] [801-555-2134] [Opratory=2,PCP=1]
                [Goldstein, Bucky] [635-45-1254] [42] [435-555-1541] [Opratory=1,PCP=1]
                [Vox, Bono] [414-45-1475] [51] [801-555-2100] [Opratory=3,PCP=2]
                The system should function with both \r\n and \n carriage return, new line configurations.


                Because this app is so small, I didn't bother to creat MVC directories.
                I didn't use String.split(), because my auto-fill says it takes a regex, which is off-limits for this assignment.
                There are no doubt other ways to accomplish this task, but without using regex, this was the most efficient way I came up with in my short time working tonight.

                Use postman to post this body to http://localHost:8080/parse
                  "Patient Name","SSN","Age","Phone Number","Status"
                  "Prescott, Zeke","542-51-6641",21,"801-555-2134","Opratory=2,PCP=1"
                  "Goldstein, Bucky","635-45-1254",42,"435-555-1541","Opratory=1,PCP=1"
                  "Vox, Bono","414-45-1475",51,"801-555-2100","Opratory=3,PCP=2"

                Thanks!
