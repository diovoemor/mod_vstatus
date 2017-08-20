My fork of
## mod_vstatus
My hack at getting it building in Visual Studio and maybe giving it a better look.
BEWARE: I know just enough C to be really dangerous. If you are brave enough to use
this fork, YOU DO SO AT YOUR OWN RISK!

##Notes:

One thing I noticed about this module when I first started using is that if you set
a ServerName with the allowed optional port assingment like;

  <VirtualHost *:443>

    ServerName www.example.com:443

    SSLEngine on

    ...

This module will list that ServerName (with port assingment) but it will never show
anything other than 0s across the board. In other words, it won't keep counts for
that particular ServerName.


