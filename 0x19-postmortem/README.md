# Postmortem


## ISSUE SUMMARY:
### DURATION OF OUTAGE:
                From point of task allocation to point of deadline

### IMPACT:
Users were unable to connect to server

### ROOT CAUSE:
                Nginx was listening to the wrong port

## TIMELINE:
### TIME DETECTED:
        Issue was detected from the point i was assigned the task(it was a task to debug      the server
### HOW IT WAS DETECTED:
        Issue was detected when trying to curl from localhost
### ACTIONS TAKEN:
        Actions taken was to check firstly if the server was running
### MISLEADING INVESTIGATION:
        Server was thought not to be running but upon futher investigation it was running

### WHO WAS IT ALLOCATED TO:
        The problem was allocated to me

### HOW INCIDENT WAS RESOLVED:
        The incident was resolved by taking a look at the configuration file of server

## ROOT CAUSE AND RESOLUTION:
### CAUSE OF ERROR:
        Server was listening to the wrong port (8080)

### HOW ERROR WAS SOLVED:
        Upon examining the config file(/etc/nginx/sites-available) it was found that the server was listening to port 8080 instead of 80.

## CORRECTIVE MEASURES:
### IMPROVEMENTS TO BE MADE:
        Properly cross check config settings when setting up server
### TODO:
        Run netstat on your terminal after setting up port to see ports connected to.
