# Q: Is 3bot secure?
Short answer: Yes. 

Longer answer: All messages transfered between the [3bot platform](https://github.com/3bot/3bot) and the [3bot-worker](https://github.com/3bot/3bot-worker) are packed, compressed and encrypted before they are transfered. 
This is done using state of the art technologies. Details and implementation can be found in [3bot-crypto](https://github.com/3bot/3bot-crypto/), the module used by the worker and the platform.
The connection to the [3bot cloud platform](https://my.3bot.io) is encrypted using SSL. 

