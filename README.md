# henry-schein-take-home-test

Assignment:

                Using best practices complete the following task:
                Create a restful web service that takes a string of CSV data as input and returns the data reformatted as
                shown below without using regular expressions or a 3 rd party CSV parser library.
                Example input string:
                
                    "Patient Name","SSN","Age","Phone Number","Status"
                    "Prescott, Zeke","542-51-6641",21,"801-555-2134","Opratory=2,PCP=1"
                    "Goldstein, Bucky","635-45-1254",42,"435-555-1541","Opratory=1,PCP=1"
                    "Vox, Bono","414-45-1475",51,"801-555-2100","Opratory=3,PCP=2"
                
                Return string for the above sample input
                [Patient Name] [SSN] [Age] [Phone Number] [Status]
                [Prescott, Zeke] [542-51-6641] [21] [801-555-2134] [Opratory=2,PCP=1]
                [Goldstein, Bucky] [635-45-1254] [42] [435-555-1541] [Opratory=1,PCP=1]
                [Vox, Bono] [414-45-1475] [51] [801-555-2100] [Opratory=3,PCP=2]
                The system should function with both \r\n and \n carriage return, new line configurations.

Solution:
                My first thought was to create a Patient object with attributes for SSN, AGE, Phone number, and Status with getters and setters, then to parse through the data                   and parse out a list of Patients. The Patient object would overwrite the toString() method, that would return a String for each value. That would have been a                     better solution if the app was expected to do more with the Patients than just return a parsed list. Becuase of the time limit, I kept it fairly simple.

                And because this app is so small, I didn't bother to creat MVC directories.
                I didn't use String.split(), because my auto-fill says it takes a regex, which is off-limits for this assignment.
                There are no doubt other ways to accomplish this task, but without using regex, this was the most efficient way I came up with in my short time working tonight.

                Use postman to post this body to http://localHost:8080/parse
                  "Patient Name","SSN","Age","Phone Number","Status"
                  "Prescott, Zeke","542-51-6641",21,"801-555-2134","Opratory=2,PCP=1"
                  "Goldstein, Bucky","635-45-1254",42,"435-555-1541","Opratory=1,PCP=1"
                  "Vox, Bono","414-45-1475",51,"801-555-2100","Opratory=3,PCP=2"

                Thanks!
