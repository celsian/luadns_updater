This bash script updates your zone records when your dynamic IP Address changes.

The script requires JQ, linux users with apt can install it with: `apt install jq`

You will need to have API Access enabled on your LuaDNS account.
Enter your details in the LuaDNS Details section starting on line 8.
ZONE_ID and RECORD_ID must be integers, not strings.

Utilize environment variables or store the script in a safe location as it contains client secrets.
Add this to a cron job that runs on a time frame of your choosing,
the logs it generates can be stored in an insecure location as they do not leak client secrets.
