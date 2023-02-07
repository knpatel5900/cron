# cron

![Set Up SSH Connections to AWS CodeCommit Repositories](https://res-1.cloudinary.com/hv4xf2jgd/image/upload/q_auto/v1/images/cron_expression_syntax.png)


## The cron command-line utility is a job scheduler on Unix-like operating systems. Users who set up and maintain software environments use cron to schedule jobs (commands or shell scripts), also known as cron jobs, to run periodically at fixed times, dates, or intervals. It typically automates system maintenance or administration—though its general-purpose nature makes it useful for things like downloading files from the Internet and downloading email at regular intervals.

Each line of a crontab file represents a job, and looks like this:

# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of the month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of the week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                   7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * * <command to execute>
The syntax of each line expects a cron expression made of five fields which represent the time to execute the command, followed by a shell command to execute.
