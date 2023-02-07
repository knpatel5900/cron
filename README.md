# cron

![Set Up SSH Connections to AWS CodeCommit Repositories](https://res-1.cloudinary.com/hv4xf2jgd/image/upload/q_auto/v1/images/cron_expression_syntax.png)


## The cron command-line utility is a job scheduler on Unix-like operating systems. Users who set up and maintain software environments use cron to schedule jobs (commands or shell scripts), also known as cron jobs, to run periodically at fixed times, dates, or intervals. It typically automates system maintenance or administration—though its general-purpose nature makes it useful for things like downloading files from the Internet and downloading email at regular intervals.

Each line of a crontab file represents a job, and looks like this:

![image](https://user-images.githubusercontent.com/59032477/217310663-56e16768-5fdb-4543-87bf-d9fc32d41264.png)

The syntax of each line expects a cron expression made of five fields which represent the time to execute the command, followed by a shell command to execute.

# Examples

## the following clears the Apache error log at one minute past midnight (00:01) every day, assuming that the default shell for the cron user is Bourne shell compliant:

    1 0 * * * printf "" > /var/log/apache/error_log
    
## This example runs a shell program called export_dump.sh at 23:45 (11:45 PM) every Saturday.

    45 23 * * 6 /home/oracle/scripts/export_dump.sh

## The below would output "hello world" to the command line every 5th minute of every first, second and third hour (i.e., 01:00, 01:05, 01:10, up until 03:55).
    
    */5 1,2,3 * * * echo hello world
