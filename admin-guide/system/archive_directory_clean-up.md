# Archive directory clean-up

The archives/ directory is used to store temporary data. XLS exports, courses backups, etc. As such, and unless you have a cron job running regularly to clean it up, you should clean it manually once in a while. This link allows you to do just that, without requiring direct access to the files directory.

The best way to clean the cache automatically for now is to install chash: https://github.com/chamilo/chash
 
> ```
> cd /tmp
> git clone -b 0.1 https://github.com/chamilo/chash
> cd chash
> composer update
> php -d phar.readonly=0 createPhar.php
> chmod +x chash.phar
> sudo mv chash.phar /usr/local/bin/chash
> ```
> 
> Then, from your cron, something like this:
> 
> ```
> 7 3 * * * root cd /web/yourchamilo/; /usr/local/bin/chash -n fct
> ```
> 
> There are many variations to this last command (notably to avoid alerts on the output of the command or to change the user executing it), but in general this should work and you can find out the rest.
> 
> If you want to know the details of Chash (which uses several stuff from Symfony), check https://github.com/chamilo/chash/blob/0.1/src/Chash/Command/Files/CleanTempFolderCommand.php#L56


