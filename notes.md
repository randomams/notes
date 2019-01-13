# ![Markdown Here logo](https://raw.github.com/adam-p/markdown-here/master/src/common/images/icon48.png)  Notes

## PIP Update all 

Apparently, pip has no build in mechanism for that.

```bash
pip freeze — local | grep -v ‘^\-e’ | cut -d = -f 1 | xargs -n1 pip install -U
```

**Note**  Use at your own risk. Some of your packages may require root privileges. Use the version below

```bash
sudo pip2 freeze — local | grep -v ‘^\-e’ | cut -d = -f 1 | xargs -n1 sudo pip2 install -U
```
