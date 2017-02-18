# Slightly evil password strength checker

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

[![](https://sr.ht/NAC4.png)](https://www.xkcd.com/792/)
