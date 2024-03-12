# healthchecks-dashboard
 
It's a standalone HTML Dashboard for Healthchecks.io service (https://healthchecks.io)

1. Fork this repo

2. Create a READ-ONLY API KEY for your healthchecks.io project:

<img width="579" alt="Captura de pantalla 2024-03-12 a las 12 08 03" src="https://github.com/johnny-tknoska/healthchecks-dashboard/assets/160315398/8861f89b-4e35-4f2e-a79b-84fdbe808881">


3. Edit the HTML file and look for this line:

         var key = "YOUR READ-ONLY API KEY HERE";    // PLACE HERE YOUR healthchecks.io project READ-ONLY API KEY //


4. Optional: The data refresh interval is set to 5 seconds by default. You can also change this setting if you want by editing this line:

         var refresh_interval = 5000;  // DATA UPDATE INTERVAL IN MILISECONDS. RECOMMENDED NOT LOWER THAN 5000 (5s) //


5. That's it! Publish or save locally your html and enjoy!  (This is my first HTML coding so be kind with me.)


<b>Features:</b>

a) This information from your checks is displayed:

- <b>Name</b>
- <b>Next within:</b> Time for the next check.
- <b>Next check:</b> Next check schedule. Time and data is displayed. Today and Tomorrow are coded for easy viewing. 
- <b>Elapsed Time:</b> Time elapsed since last check
- <b>Last check:</b> Last check schedule. Yesterday and Today ared coded for easy viewing.
- <b> # pings:</b> Number of pings
- <b> Running time:</b> for those jobs with /start function displays the last running time

- For <b>Next within and Elapsed time</b>, these rules apply:

            If time is < 1 min, seconds are displayed
            If time is < 1 hour, minutes and seconds are displayed
            If time is < 1 day, hours and minutes are displayed
            If time is > 1 day, days, hours and minutes are displayed

- For <b>Next within and Next check</b>, this rule applies:

           If the expected time between checks (check schedule, period) exceeds 300 days,
           > 300 days is displayed in Next check and Next within.

<img width="567" alt="Captura de pantalla 2024-03-12 a las 11 19 39" src="https://github.com/johnny-tknoska/healthchecks-dashboard/assets/160315398/50c276a6-d480-4c8c-b663-8f36c95012d8">


b) You can order the information displayed by Name, Next check, Last check, pings and Running Time is ascending/descending order.


c) Color coding:

        If a check is on time, the Name cell is green.
        If a check is in grace period, Name and Next within cells are orange.
        If a check is down, Name,Next within and Next check cells are red; also "down" is displayed at Next within cell.

<img width="595" alt="Captura de pantalla 2024-03-12 a las 12 30 20" src="https://github.com/johnny-tknoska/healthchecks-dashboard/assets/160315398/b3f219a5-ede5-42cc-a2e6-a7f69a3ba223">








