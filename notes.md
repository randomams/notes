= Notes

== PIP Update

Apparently, pip has no build in mechanism for that. This is why I have decided to provide this simple one-liner,

pip freeze — local | grep -v ‘^\-e’ | cut -d = -f 1 | xargs -n1 pip install -U

**Note**  Use at your own risk. Some of your packages may require root privileges. Use the version below

sudo pip2 freeze — local | grep -v ‘^\-e’ | cut -d = -f 1 | xargs -n1 sudo pip2 install -U


```javascript
alert('test syntax highlighting.');
```
