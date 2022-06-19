Follow these steps to run the conatiner:


create a workspace dir
mkdir /ws



Also, perform the below tasks on it:
1. Mount a volume containing an HTML webpage with "Hello World!" message in it
2. Replace the default welcome page of Nginx with the HTML page from step 1
3. Modify Nginx configuration to capture client IP address in the log.
4. Capture the Nginx access log & error log in the docker stdout & stderr