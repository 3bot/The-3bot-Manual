# Q: Can I use 3bot with Github or Bitbucket?
Yes, if you're using the [3bot cloud platform](https://my.3bot.io) everything is ready to go. Check the "hooks" tab on the workflow and set it up for external services. If you're running your own instance, check the [3bot-hooks](https://github.com/3bot/3bot-hook) module. 

Once set up, 3bot will perform (execute the workflow) when you push to the repostory connected.

# Q: Is 3bot secure?
Short answer: Yes. 

Longer answer: All messages transfered between the [3bot platform](https://github.com/3bot/3bot) and the [3bot-worker](https://github.com/3bot/3bot-worker) are packed, compressed and encrypted before they are transfered. 
This is done using state of the art technologies. Details and implementation can be found in [3bot-crypto](https://github.com/3bot/3bot-crypto/), the module used by the worker and the platform.
The connection to the [3bot cloud platform](https://my.3bot.io) is encrypted using SSL. 

