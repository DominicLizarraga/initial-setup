# Always read what the Terminal throws you. ⛔️

if `pg` fails, then run - `brew install libpq`

```bash
# Add the following line to your ./zshrc file
export PATH="/opt/homebrew/opt/libpq/bin:$PATH"
```

One big proble we faced was that Ruby version was not being called when we ran `ruby -v`.

The reason? an issue on how the directories were organized. How they initially got installed.

Finally we ran `gem environment` to see the whole directory.

Moved one “.gem” file from its original location to the where it should be (still don’t know what created it), and then we deleted the “.gembk” (weird directory)
