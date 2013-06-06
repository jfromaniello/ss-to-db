Only for MAC OSx.

Send screenshot to Dropbox. 

> Want to upload to s3? use this other one [ss-to-s3](http://github.com/jfromaniello/ss-to-s3).

## Install

	npm install ss-to-db -g

First time you run it, a browser window will open prompting access to your dropbox. Next time it will read the access token from `~/.ss-to-db`.


## Usage

Run `ss-to-db` from the terminal or create a service with Automator and assign a shortcut as described in the next section.


## Create a shortcut

First you will need to create a __SERVICE__ with automator. Select "run shell script" in Actions and then write `/usr/local/bin/ss-to-db` as shown here (replace s3 with db):

![ss-2013-06-04T09-44-23.png](http://blog.auth0.com.s3.amazonaws.com/ss-2013-06-04T09-44-23.png)

Next you will asign a key shortcut to the service, in System Preferences as shown here:

![ss-2013-06-04T09-27-26.png](http://blog.auth0.com.s3.amazonaws.com/ss-2013-06-04T09-27-26.png)

You are done! close Automator and System Preferences before testing.

## Better global shortcut

The above instructions use OSx Services, which doesn't work on every program but most of them. The other way I've found is by creating an Application with Automator (instead of a Service) and then using any of these tools to create the key shortcut:

Alfred, Apptivate, BetterTouchTool, Butler, iKey, Keyboard Maestro, KeyLauncher, Keymando, Launch it!, NuKit, Quickeys, Quicksilver, RocketShip, Shortcuts, Spark, Twitch

Thanks to this [answer in stackoverflow](http://apple.stackexchange.com/a/20116/50602).

## License 

MIT - 2013 - José F. Romaniello