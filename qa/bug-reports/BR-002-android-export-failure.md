# Bug Report BR-002

## Title

Android APK Export Failure - ERR_CONNECTION_REFUSED

## Environment

* Windows 11
* HTML, CSS and JavaScript project
* Android APK export process

## Severity

High

## Problem Description

During the APK export process, the application consistently failed to run correctly and displayed the error:

ERR_CONNECTION_REFUSED

The issue prevented the application from launching successfully on Android devices.

## Initial Investigation

At first, I suspected that the problem was related to the APK packaging tools or a bug in the application code.

I reviewed multiple parts of the project, including:

* APK export configuration
* HTML structure (index.html)
* JavaScript files
* CSS files
* Project settings

Several potential fixes were tested, but the problem remained unresolved.

## Root Cause Analysis

During further investigation, I considered the possibility of a file naming issue.

I learned that Android relies on a Linux-based file system, which is case-sensitive. Unlike Windows, file names with uppercase and lowercase letters are treated as different files.

The project contained files with uppercase letters in their names, including:

* Game.js
* Index.html
* Style.css

Some file references did not match the exact capitalization of the actual files.

## Solution

All file names and references were standardized using lowercase naming conventions:

* game.js
* index.html
* style.css

After updating the file names and references, the project was exported again.

## Result

The APK export completed successfully and the application launched correctly on Android devices.

## Lessons Learned

* Linux-based systems are case-sensitive.
* File naming consistency is critical when deploying across different operating systems.
* Troubleshooting should include environmental and platform-specific factors, not only application code.
* Taking time to step back and review assumptions can help identify root causes more effectively.

## Skills Demonstrated

* Troubleshooting
* Root Cause Analysis
* Cross-Platform Compatibility
* Software Testing
* Technical Research
* Problem Solving
