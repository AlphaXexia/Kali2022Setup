# Kali2022Setup
A Simple Kali Setup in 2022
<ol>
  <li>
      
## Create a new user
  This would allow you to have your own username rather than using the default users, and also more helpful for you to learn when it comes to priveleged and unprivelged users.
```
# Create your user
~$  adduser {preferred_username}

# add priveleges to user
~$  usermod -aG sudo {preferred_username}

# change the default user credentials(root & kali)
~$  cd /etc/ssh
~$  passwd {default users}
```
  Once you've finished that it's time to switch users, you may log out and choose your new user.

  </li>
  <li>
    
## Install, Update & Upgrade
  This sets you up on what you up on your basic necessities in practicing offensive cybersecurity.

But before starting to install any packages make sure to update your machine first.
```
~$  sudo apt update -y
```

If you have trouble deciding which packages to install you can take your pick based on what you want to do using [this][1].
    
[1]: <https://www.kali.org/docs/general-use/metapackages/> "Kali Linux Metapackages"
```
~$  sudo apt-get install yakuake docker git openvpn apt-utils kali-linux-default kali-tools-web -y
```

  </li>
  <li>
    
## I dont know how to make **CRON Jobs** yet

*CRON Jobs* are basically commands that you give to your machine to perform automated tasks, for example is running an application once a specific trigger is activated like a user signing in. And here comes the fairly easy part, proceed to search from your list of programs the *Session and Startup* and proceed to add applications that you would prefer to launch based on session status.

    Will show a gif soon

  </li>
<li>
  ## Early Session Signout

We can be honest with each other, it's pretty annoying that when you want to check something on your host OS sometimes would get signed out of your Guest OS on your virtualbox. Which for a fair reason a good prevention for anyone else to snoop into your private stuff. but if you still want to fix that you can search from your list of programs the *Power Manager*. In which you can configure what would hapen since inactivity in your Guest OS.
</li>
</ol>
