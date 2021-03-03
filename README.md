# Install TuxSuite

This will create `~/bin/tuxsuite`.

```
pip3 install -U --user tuxsuite
```

# Create Config

```
mkdir -p ~/.config/tuxsuite
echo "[default]" > ~/.config/tuxsuite/config.ini
echo "token=XXXXYYYYYYZZZZZZZZZ" >> ~/.config/tuxsuite/config.ini
```

# Run Full Set

```
tuxsuite build-set \
    --git-repo 'https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux-stable-rc.git' \
    --git-ref queue/5.11 \
    --tux-config all.yaml \
    --set-name all
```
