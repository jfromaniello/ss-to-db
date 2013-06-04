Only for MAC OSx.

Send screenshot to Amazon S3.

## Install

	npm install ss-to-s3 -g

Then you need to create a `~/.ss-to-s3.config` file with something like this:

~~~javascript
{
	"ACCESS_KEY_ID":     "MY-ACCESS-KEY",
	"ACCESS_KEY_SECRET": "MY-KEY-SECRET",
	"BUCKET":            "THE-BUCKET",
	"COPY_FORMAT":       "![{filekey}](http://THE-BUCKET.amazonaws.com/{filekey})"
}
~~~

ACCESS KEY, SECRET and BUCKET are the Amazon S3 parameters, COPY_FORMAT is a mask of what is going to by write to your clipboard after finished.

## Usage

Run `ss-to-s3` from the terminal or create a service with Automator and assign a shortcut as described in the next section.


## Create a shortcut

First you will need to create a __SERVICE__ with automator. Select "run shell script" in Actions and then write `/usr/local/bin/ss-to-s3` as shown here:

![ss-2013-06-04T09-44-23.png](http://blog.auth0.com.s3.amazonaws.com/ss-2013-06-04T09-44-23.png)

Next you will asign a key shortcut to the service, in System Preferences as shown here:

![ss-2013-06-04T09-27-26.png](http://blog.auth0.com.s3.amazonaws.com/ss-2013-06-04T09-27-26.png)


You are done! close Automator and System Preferences before testing.

## License 

MIT - 2013 - José F. Romaniello