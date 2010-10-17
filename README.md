Gem Skeleton for use with Bones
===============================

# Overview

When creating a new gem for a Ruby library, it's nice to have a solid starting
place, from which you can modify and build on to get your library up and
running more quickly.

Mr Bones is a tool that allows just such a startup environment, but the
default skeleton (template) that it uses [is non-ideal][1] because it locks
you in to always requiring Mr Bones itself. This skeleton aims to alleviate
that concern by providing a nice, clean and independent skeleton for the
creation of new gems.

 [1]: http://iampedantic.com/posts/FIXME

This skeleton assumes use of Git and RSpec 2. Feel free to modify it to your
own needs if you don't use these tools.

# Usage

First, you'll need Mr Bones installed:

    $ gem install bones

(Side note: if you're using `sudo` to install your gems, you're doing it
wrong. See [Homebrew's notes on Gems, Eggs and Perl Modules][2]).

 [2]: http://github.com/mxcl/homebrew/wiki/Gems,-Eggs-and-Perl-Modules

Then you'll want to “freeze” this skeleton in your install of Mr Bones, so
you can use it to create new gems. I'm naming the skeleton 'rspec2', but you
can name it whatever you want.

    $ bones freeze -r git://github.com/h3h/bones-skeleton-rspec2.git rspec2

Lastly, just use `-s rspec2` when creating a new library with bones and you're
done:

    $ bones create -s rspec2 mynewlib

# Inspiration

This skeleton was inspired by both Tom Preston-Werner's [RakeGem][3] and the
default [Mr Bones][4] skeleton.

 [3]: http://github.com/mojombo/rakegem
 [4]: http://github.com/TwP/bones

# License

This skeleton is distributed under the MIT License, as mentioned in the
`LICENSE` file.
