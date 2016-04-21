# rev-door
**rev-door** is a small backdoor with only ONE line of PHP code, which takes command from POST data and execute it on server side. It is like other simple GET based backdoor but the only difference is it uses POST request to receive commands.


The difference
-----
The regular GET backdoors are executed with get request like <code>http://www.example.com/get.php?cmd=ls -la</code>
But this backdoor cannot be executed by this way, thus it is more secure in a sense to use because at first glance (at least to me) it seems useless backdoor.
The link is just <code>http://www.example.com/post.php</code>. No GET parameter.

So how to use it?
-----
I think you have Mozilla Firefox and [HackBar](https://addons.mozilla.org/en-US/firefox/addon/hackbar/) addon ready.

* Now go to your backdoor link. (in my case it is <code>http://localhost/ss.php</code>)
* Then on HackBar click Load URL
* Then tick the **Enable Post data**
* Now in the **Post Data** textbox write <code>commandz=ls -la</code>  (Because the POST request parameter is "commandz" in the backdoor script)
* Now click **Execute**

*You see the result?????*
That's it! 



![Demo](http://i.imgur.com/CW5xDlN.png "Demo Image")
