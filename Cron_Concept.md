# Concept of Cron

Cron is a time-based job scheduler in Linux.

It automatically executes scripts or specific commands at configured times.

In a crontab entry, the schedule is written in the order: minute, hour, day of month, month, and day of week. An asterisk (*) means “every” possible value for that field.

For example:`* * * * * echo "Hello"` (run echo "Hello" every minute.)