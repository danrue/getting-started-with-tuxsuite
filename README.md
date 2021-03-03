# Install TuxSuite

This will create `~/bin/tuxsuite`.

```
pip3 install -U --user tuxsuite
```

# Create Config

Look for "Welcome to TuxBuild" email for a token.

```
mkdir -p ~/.config/tuxsuite
echo "[default]" > ~/.config/tuxsuite/config.ini
echo "token=XXXXYYYYYYZZZZZZZZZ" >> ~/.config/tuxsuite/config.ini
```

# Run Full Set

Run ~232 builds in parallel.

```
tuxsuite build-set \
    --git-repo 'https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux-stable-rc.git' \
    --git-ref queue/5.11 \
    --tux-config all.yaml \
    --set-name all
```

# Questions

Documentation can be found at [docs.tuxsuite.com](https://docs.tuxsuite.com/).

The TuxSuite team may be engaged through chat, email, or gitlab issues.

To chat with us, [join our public Discord](https://discord.gg/4hhTzUrj5M), or
our IRC channels #tuxsuite and #tuxmake on
[freenode.net](https://freenode.net/).

Questions, comments or feedback are always welcome by private email at
tuxsuite@linaro.org.

Finally, gitlab issues are used to track bugs and feature requests in both
[tuxsuite](https://gitlab.com/Linaro/tuxsuite/-/issues) and
[tuxmake](https://gitlab.com/Linaro/tuxmake/-/issues) projects.
