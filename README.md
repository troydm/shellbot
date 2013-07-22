shellbot
========

Potentialy unsafe IRC bot that can remember and remotely execute shell scripts on your server. 
Written in Perl 5 using excellent [POE::Component::IRC](https://metacpan.org/module/POE::Component::IRC) framework 
and supports only *nix operating systems (Linux, Solaris, BSD)

install
-------

    cpanm POE::Component::IRC Time::SoFar YAML Proc::Daemon Time::Piece
    git clone git@github.com:troydm/shellbot.git
    mv ./config.example ./config

Optional (to connect using SSL)

    cpanm POE::Component::SSLify
    

configure
---------

edit config file and specify your irc network server and port and bot nick
you can also uncomment some of the options that you might want to change.
Also make sure you'll add your full irc name to authorizations list, 
otherwise you won't be able to command the bot

run
---

    chmod +x ./shellbot
    ./shellbot ./config 

how to use
----------

private message the the bot for help.

    /msg botnick help


