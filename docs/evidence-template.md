# Week 7 Evidence

Student Name: Mei Morrow
Repository URL: https://github.com/Mei-Morrow/sdi4213-week7.git
Pull Request URL: https://github.com/Mei-Morrow/sdi4213-week7/pull/2

Note: All eight screenshots and captions are provided in the evidence document submitted on Canvas.

## Screenshot 1 — Local Help Desk Application
The Service Request Tracker runs locally with SQLite. The visible “Printer not working” request confirms that a service request was successfully created and displayed.

## Screenshot 2 — Docker Compose Services Running
Docker Compose shows the web, PostgreSQL, and Adminer services running. PostgreSQL reports a healthy status, confirming that its readiness check passed.

## Screenshot 3 — Help Desk Requests and Status Update
The Docker-hosted Help Desk application displays two distinct service requests. The printer request was updated to “In Progress,” demonstrating request creation and status updates.

## Screenshot 4 — PostgreSQL Records Viewed in Adminer
Adminer displays the two service requests stored in PostgreSQL, including the updated “In Progress” status. This confirms that the web application saves its records in the database.

## Screenshot 5 — Requests Persist After Container Replacement
The same two requests and their statuses remain after running docker compose down and docker compose up -d. The named PostgreSQL volume preserved the records while the containers were removed and recreated.

## Screenshot 6 — Web Service Logs
The web service logs show Streamlit’s startup output from the Docker container. These logs provide a way to inspect service activity and troubleshoot startup problems.

## Screenshot 7 — Database Reset After Volume Deletion
After running docker compose down -v and restarting the services, the previously created requests are no longer present. Removing the named PostgreSQL volume deleted the stored database data.

## Screenshot 8 — Final Pull Request with Passing CI
The final pull request shows a passing CI check for the Week 7 Help Desk application. The repository and branch information identify the changes being merged into main.

Note: Reflection exception given by instructor.
## Reflection
1. Why does the web service use `db` instead of `localhost`?
2. What problem does the named volume solve?
3. What is the difference between `docker compose down` and `docker compose down -v`?
4. What was the most difficult part of the exercise?
