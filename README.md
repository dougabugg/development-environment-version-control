# development-environment-version-control
Track changes to a developement environment

At the very least, the source code for an application is tracked in version control software like git. Less often are changes to the development environment itself tracked. Usually, it isn't necessary to track environment changes, but for some code bases, troubleshooting failing local builds can be a large enough task that it might be beneficial to track all the changes made to the dev environment as part of doing development on that code base.

I few ideas of features to have. Changes to the following systems would be monitored and tracked by an external application.
- environment variables
- build tool configuration files
- files flagged by gitignore

The reason for tracking files in gitignore, is that some files shouldn't have their changes tracked with the source code, but may still cause the build to fail if they aren't manually cleaned out. Although setting up the files to be automatically cleaned would be a better solution, when troubleshooting a build failing during development, being able to track changes to them can be helpful.
