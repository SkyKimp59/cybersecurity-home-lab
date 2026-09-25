# Linux Log Analysis Lab

## Objective

Learn basic Linux command-line navigation and practice searching
through authentication logs.

## Environment

- Host: Apple M3 Mac
- Virtualization: UTM
- Operating System: Ubuntu 26.04.1 LTS
- Lab type: Virtual machine

## Skills Practiced

- Navigating the Linux filesystem
- Creating directories with `mkdir`
- Creating/editing files with `nano`
- Viewing files with `cat`
- Searching text with `grep`
- Basic security log analysis

## Lab Setup

Created a working directory:

    /home/myname/cyberlab

Created a sample authentication log:

    login.log

## Commands Used

    pwd
    ls
    cd
    mkdir
    nano
    cat
    grep

## Investigation

Used `grep` to search the log for:

- Failed login attempts
- Successful login attempts
- Specific usernames
- Specific IP addresses

## What I Learned

Linux provides command-line tools that can be used to
search and analyze security-related logs.

This exercise introduced the basic workflow of identifying
relevant events and filtering log data for investigation.
