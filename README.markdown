These are my bash configuration files. In order for them to work, you need to source the `<your_path>/dotfiles/bashrc` file in your `~/.bashrc`

    if [ -f <your_path>/dotfiles/bashrc ]; then
      . <your_path>/dotfiles/bashrc
    fi

Also, if you have a `~/.bash_profile` you can put the next code in it to source `~/.bashrc`

    if [ -f ~/.bashrc ]; then
      . ~/.bashrc
    fi

Finally, in my PS1 I call the vcprompt script wich is used to display the working git branch on your prompt. Here's the download:

    wget http://vc.gerg.ca/hg/vcprompt/archive/tip.tar.gz && tar zxvf tip.tar.gz && cd vcprompt-07f110976599/ && make && cp -p vcprompt ~/bin && cd .. && rm -rf tip.tar.gz vcprompt-07f110976599/
