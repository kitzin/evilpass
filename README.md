# Slightly evil password strength checker (ORIGINALLY FORKED FROM SIRCMPWN BEFORE HE REMOVED GITHUB ACCOUNT?) see [https://git.sr.ht/~sircmpwn/evilpass](https://git.sr.ht/~sircmpwn/evilpass)

Checks how strong your user's password is via questionably ethical means.

![](https://sr.ht/sHst.gif)

## Usage

Please don't actually use this.

```python
>>> from evilpass import check_pass
>>> errors = check_pass("password", "email address", "username")
>>> errors
["Your password must be at least 8 characters long"]
```

## Password reuse is bad, okay?

So quit doing it. Use a password manager. I personally recommend
[pass](https://www.passwordstore.org/).

## Side note

If you're actually checking user's password strength on sign up, I strongly
suggest using a minimum entropy instead of contrived rules like this. I also
suggest not trying to log into your user's account on other sites.

## Future development

* Automate use of proxies to avoid rate limiting and other things external
  services might do when they detect you're doing this
* Add other external services to check (I spent about 5 minutes on Google before
  I decided it wasn't worth the time required to reverse engineer their login
  flow, but it might be the most valuable account to try)
* ~~Store valid credentials in a database for evil purposes~~

https://www.xkcd.com/792/
