DevShop Source
==============

This repo is nothing but git submodules to all of the devshop-related 
open source projects.

This repo is very helpful when developing for devshop, since there are so many 
inter-related projects in different repos.

This is also helpful if you want to update all of the projects at once to the 
latest code.

To use this repo, clone it and then update the submodules.

  $ git clone git@github.com:thinkdrop/source.git
  $ cd source
  $ git submodule init
  $ git submodule update

Once the source is in place, it may be useful for you to use symbolic links to allow 
your aegir/devshop server to use the code from ~/source.


To put DevShop Hosting into hostmaster:

$ ln -s /var/aegir/source/devshop_hosting /var/aegir/hostmaster-6.x-1.x/sites/all/modules

To put DevShop Provision into Drush:

$ ln -s /var/aegir/source/devshop_provision /usr/share/drush/commands/

Coming soon: setup.sh
