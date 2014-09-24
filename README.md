bitcasad
========

bitcasad is a commandline daemon/guard to automount your bitcasa linux account 
and keep it connected watching periodically.


Installation
------------

    wget https://github.com/falcacibar/bitcasad/blob/master/bitcasad -O /usr/local/bin/bitcasad
    chmod 755 /usr/local/bin/bitcasad
    
    
Configuration
-------------

bitcasad reads the accounts from a credentials file, like this.


    [/home/me/Bitcasa]
    account=my.bitcasa@account
    password=mysupersecretpassword
    
    
The file could be one of this paths:

* `/etc/bitcasa.ini`
* `$HOME/.bitcasa/credentials.ini`


Add to session Startup
----------------------

##### Unity and Gnome
- Press `Alt`+ `F2`and type `gnome-session-properties`
- Click Add
- Fill with <br>
    **Name**:`bitcasad`                            
    **Command**:`/usr/local/bin/bitcasad`


Checking if all it's OK
-----------------------

- Launch a terminal (In Unity/Gnome by pressing `Ctrl`+`Alt`+`T` Keys)
- Run the `bitcasad` command (just typing `bitcasad` and pressing `Enter`)
- Check the output error for details, don't exit, credentials files will 
  be re-readed , so edit the credentials file and see the terminal again.
- Exit by pressing `Ctrl`+`C`


Ready... Go!
-----------------

Launch `bitcasad` manually the first time (With `Alt`+`F2` for example) 
and enjoy.