The 3bot Manual
===============


3bot is an open-source software platform backed by arteria GmbH to build, configure and perform.
To "perform" is the general term for remote executing tasks by running workflows.
These could be configuration management (CM), continuous integration (CI), continuous delivery (CD) or application deployment
tasks but also allows you to re-use your shell scripts in a fast and efficient way from a central point.


# Exploring and using 3bot

There are two version of the 3bot, the [3bot cloud a free to use SaaS version](https://my.3bot.io) of 3bot or the self hosted 3bot instance. These are a few things (workflows) that can be done with 3bot:
 
* Create/Setup new Django projects (server configuration, basic installation with pip, repository creation on BitBucket, ...)
* Deploy a project when changes are pushed to a repository, requires [3bot-hooks](https://github.com/3bot/3bot-hook) for the self hosted version. 
* Create Python packages (file structures using [cookiecutter](https://github.com/audreyr/cookiecutter), repo on BitBucket, ...)
* Do Continuous Integration and releasing software (Git Flow approach)
* Running Tests (Test Runner, Selenium, ...)
* Releasing Python packages on your own or the global package index.
* ... 

Basically you could do whatever you want with it, especially what is boring to repeat. 

The idea is not to replace tools like Travis, Jenkins, Salt, etc. but to connect them all together if you use them.


## The 3bot cloud 

### Getting an invite for the 3bot cloud

There is a cloud version of 3bot that can be found [here](http://my.3bot.io). [Ask for an invitee](https://www.arteria.ch/de/#about-form-lead)!

### Once You Got Invited

Accept the invitation and create your account. Once you're in you're part of the global 3bot team as well. There you can clone (steal, get inspired, .. by) tasks. 

Next will be to [setup a worker](https://github.com/3bot/3bot-worker/blob/master/README.md) on a server or on your laptop. The worker must be accessible from the web, please update the firewall accordantly.    

### Inviting others and create more teams 


## Setting up your own 3bot 

See [QUICKSTART.md](https://github.com/3bot/3bot/blob/master/QUICKSTART.md) in the platform repository for more information how to set up your own instance of 3bot. A lot of the process described in "The 3bot cloud" earlier in this document applies to the self hosted version as well. 


# Best Practices
## Best Practices for Django development

What we learned when using 3bot when working with [Django](https://www.djangoproject.com/):

    * Install a worker on each server you have and ..
    * install a worker in every virtualenv you use as well. This allows to re-use workflows for all envs without modifying them. The global worker can be used to update the worker running in the envs distributed on the system. 
    * Use [virtualenv-mgr](https://github.com/arteria/virtualenv-mgr) to do the update/locate/.. virtualenv automagic. 


    
 
# Team
## Team Members
## Team Admins
Team Admins are regular Team Members but has extended privileges. 
* Only Team Admins can edit Read Only tasks.
* ..


# Invite others to use 3bot

## Add a member to a team

1. In the profile dropdown on the top right (your name) choose the team where you want to add members.
2. Press the "Add a member" button.
3. Fill the form
    * ``Email`` is the email address of the new team member. An invitation link will be sent.
    * ``Is admin`` is optional. Go to the [admin section]() for details about admin privileges.  

## Create a new team for someone

Invite others by creating an organization for them. You will not be part of the new team.

1. In the profile dropdown on the top right (your name) choose "Create new Team".
2. Fill the form
    * ``Name``, eg. "Dummy Ltd.", the name to be displayed. 
    * ``Slug``, eg. "dummy-ltd", a lowercase name (optional with hyphens) suitable for unique identification
    * ``Email`` is the email address of the new team owner. An invitation link will be sent.
