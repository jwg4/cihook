# cihook
Do builds and stuff whenever you push stuff.

## How to use it.

To use cihook, you have to add the generic on-push hook script to your git server, and it has to be able to run, which means it must be able to import the cihook package. Installing cihook globally on the git server is probably enough, although you might want to install it in a different way.

Everything else happens through git. You can add the file .cihook to your repository and the hook script will look at it and figure out what to do.

Logs, outputs and artefacts of your builds will be committed to git, either in a generic repo which holds results of all your builds, in a new repo just for your project, or in the project repo itself. You can open a html file which will show you all that data, and which will dynamically update when more results are pulled.

Configuration of the CI server works the same way. Clone the cihook_config repo and make changes, then push them.
