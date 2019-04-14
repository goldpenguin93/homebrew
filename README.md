# Homebrew Start #

## macOS ##

### copy and paste into terminal. ###

```terminal

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

```
### Homebrew installs ###

```

$ brew install wget

```


### Homebrew won’t install files outside its prefix and you can place a Homebrew installation wherever you like. ###


```

$ cd /usr/local
$ find Cellar
Cellar/wget/1.16.1
Cellar/wget/1.16.1/bin/wget
Cellar/wget/1.16.1/share/man/man1/wget.1

$ ls -l bin
bin/wget -> ../Cellar/wget/1.16.1/bin/wget

```

### Trivially create your own Homebrew packages. ###


```

$ brew create https://foo.com/bar-1.0.tgz
Created /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core/Formula/bar.rb

```

###  It's all Git and Ruby underneath, so hack away with the knowledge that you can easily revert your modifications and merge upstream updates.  ###


```

$ brew edit wget 

```




