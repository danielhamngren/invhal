+++
date = "2019-03-20T22:42:00+01:00"
title = "A new Idea"

+++
I had a new Idea. What would be cool would to be able to log and analyze everything in your terminal history.

Step one is to have timestamps for the history entries. Bash and zsh has support out of the box for this.

Step two is to be able to sync the histories between terminals, I always use tmux and has at least couple terminals running at the same time. Bash doesn't handle this well, but zsh do. This might be the feature that will make the switch to zsh worthwhile.

Step three is to sync the histories between different computers. This could be the tricky but also interesting part. I have been playing with the thought of using peer2peer tech for this part. I essentially only need a distributed write only log. I could have a node script running updating the log and syncing it with other actors. This node script would be instantiated with

    npx disthist --key [key]

from within .zshrc. (Maybe that would work)

Step four is to have a analysis engine that through visualizations display active time in the terminal, most used commands, most used sequences, suggestions for automation. 