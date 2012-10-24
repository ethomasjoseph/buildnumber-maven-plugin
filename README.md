What Build Number Maven Plugin
================================
This mojo is designed to get a unique build number for each time you build your project. So while your version may remain constant at 1.0-SNAPSHOT for many iterations until release, you will have a build number that can uniquely identify each build during that time. The build number is obtained from scm, and in particular, at this time, from svn. You can then place that build number in metadata, which can be accessed from your app, if desired.

The mojo also has a couple of extra functions to ensure you get the proper build number. First, your local repository is checked to make sure it is up to date. Second, your local repository is automatically updated, so that you get the latest build number. Both these functions can be suppressed, if desired.

Optionally, you can configure this mojo to produce a revision based on a timestamp, or on a sequence, without requiring any interaction with an SCM system. Note that currently, supported SCMs are : subversion, git and mercurial.

## Project Origin

This is a clone of buildnumber-maven-plugin project from Codehaus repo at http://svn.codehaus.org/mojo/trunk/mojo/buildnumber-maven-plugin

This repository has been cloned with the following command:

	git svn clone http://svn.codehaus.org/mojo/trunk/mojo/buildnumber-maven-plugin --no-metadata -A authors-transform.txt --no-minimize-url --trunk=http://svn.codehaus.org/mojo/trunk/mojo/buildnumber-maven-plugin --branches=http://svn.codehaus.org/mojo/branches --tags=http://svn.codehaus.org/mojo/tags buildnumber-maven-plugin

where authors-transform.txt can be created as explained at http://john.albin.net/git/convert-subversion-to-git

