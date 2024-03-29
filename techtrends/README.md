# TechTreds Web Application

This is a Flask application that lists the latest articles within the cloud-native ecosystem.

## Run 

To run this application there are 2 steps required:

1. Initialize the database by using the `python init_db.py` command. This will create or overwrite the `database.db` file that is used by the web application.

2.  Run the TechTrends application by using the `python app.py` command. The application is running on port `3111` and you can access it by querying the `http://127.0.0.1:3111/` endpoint.
    * If using a VM with a private network and static IP address, use the static IP address in place of 127.0.0.1 to access it from the host machine's browser. In the current case, as per the Vagrantfile, the IP address is 192.168.56.0 so the endpoint to query would be `http://192.168.56.0:3111/`
    * To separately check the output logs and error logs, try the following
      ```
      # Run the app displaying only stdout but logging both stdout and stderr separately
      python app.py 2> stderr.log 1> >(tee stdout.log)

      # Verify if the logs are identical; the initial startup messages printed in stdout will be the only difference
      sdiff -s stdout.log stderr.log
      ```
