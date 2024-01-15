# Bandit0

## Level goal
The goal of this level is for you to log onto the game server using SSH. The host that you need to connect to is *bandit.labs.overthewire.org*, on port 2220. The username is *bandit0* and the password is *bandit0*. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Logic
We just need to connect to a host using SSH with the following credentials,  
**Host**: bandit.labs.overthewire.org

**Port**: 2220

**Username**: bandit0

**Password**: bandit0

~~Note: When already connected to *bandit.labs.overthewire.org* we can just change user for the *localhost* like so,   ~~  
~~```ssh bandit1@localhost``` ~~  

Looks like connecting from *localhost* is now blocked to conserve resources so the above will no longer work

## Commands
```ssh bandit0@bandit.labs.overthewire.org -p 2220```
