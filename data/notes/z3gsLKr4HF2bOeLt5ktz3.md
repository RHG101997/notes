
## Chirpy Jekyll theme

The theme `Chripy` is used on the main page of my site, it is a static website mainly for blogging, uses markdown to create notes and other. But I will use it mostly for the front, and notes will be written only on Dendron.

https://github.com/cotes2020/jekyll-theme-chirpy

This theme is used mostly for proffessional writting, but in my case I just want a canvas to write ideas/code snippets that will be used for me later on. Cheatsheets, tips, and other important information.

### Running Website Locally

Download and install jekyll using:


```console
$sudo apt-get install ruby-full build-essential zlib1g-dev
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
gem install jekyll bundler
```

And then execute to install all the gems needed for the theme.:

```console
$ bundle
```

To run the page using docker which is easier and requires less installation run the following in linux:

```

$ docker run -it --rm \
    --volume="$PWD:/srv/jekyll" \
    -p 4000:4000 jekyll/jekyll \
    jekyll serve

```