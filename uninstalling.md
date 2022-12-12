## Uninstalling `rbenv`

```bash
rvm implode && sudo rm -rf ~/.rvm
sudo rm -rf $HOME/.rbenv /usr/local/rbenv /opt/rbenv /usr/local/opt/rbenv
brew remove rbenv
rm -rf ~/.rbenv
```

## Uninstalling `ruby`

Where is ruby installed?
`which -a ruby` or `whereis ruby`

Uninstalling all ruby dependencies with brew; this will show you all ruby files

`brew list`

To remove all ruby

`brew uninstall --force ruby`

To remove all unused dependencies

`brew autoremove`

By this time you should only see ruby-build and I deleted with:

```bash
brew uninstall rbenv
brew uninstall ruby-build
rm -rf $HOME/.rbenv
exec $SHELL -l 
cd $HOME
\curl -sSL https://get.rvm.io | bash -s stable --ruby=2.1.2
source $HOME/.rvm/scripts/rvm
```

No ruby signal… 

To check that ruby is not found 🔎

`brew list ruby` you should see an error:

`Error: No such keg: /opt/homebrew/Cellar/ruby`

## Uninstalling gems (only LOCAL gems left) 𝌤


`gem list` (will show all gems installed)

```bash
gem uninstall --all

sudo gem uninstall -aIx (in case it says you don’t have permission)

gem clean
```

## Uninstalling Rosetta 2

Follow this [link](https://iboysoft.com/news/uninstall-rosetta-2.html)

Remember nowadays is not needed to run your machin with Rosetta2. Please do not install it. 💾
