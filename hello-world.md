# Hello World

This how to applies to the [3bot cloud](http://my.3bot.io) and shows how to download a dummy image form [lorempixel.com](http://lorempixel.com/). This may be different form the self hosted 3bot in some points.

* After that your worker is up and running (accesible), you could [clone this task](https://my.3bot.io/task/1-40-download-a-placeholder-image/) from 3bot to your own team.
* Use the wheel on the right side and select "Clone for _your team_" .
* Once done, go the the fresh cloned task that belongs to _your team_ now. 
* Again click on the wheel and select "New Workflow". This creates a [workflow](https://github.com/3bot/The-3bot-Manual/blob/master/workflow.md) containing the cloned task. 
* Select your worker and press "Perform". 
* You will be prompted to enter an image path. ![Prompt asking for an image path](https://www.arteria.ch/media/imgbucket/Screen_Shot_2015-07-15_at_13.33.27.png) The path must have an ``.jpg`` extension, /tmp/dummy.jpg should work if you are on Linux, Mac OS X .., however, the path must be writable. 
* Second prompt, choose your image size, eg 200 for 200x200 pixel.
* Now the workflow and it's tasks will be executed on the worker. You will find a /tmp/dummy.jpg on your disk.
* Standard out will be captured as console output, stderr as error stream. ![](https://www.arteria.ch/media/imgbucket/Screen_Shot_2015-07-15_at_13.35.34.png) 
