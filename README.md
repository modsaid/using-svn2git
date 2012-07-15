using-svn2git
=============

A quick way to get svn2git working directly with the least commands, by having the needed dependecies in a Gemfile

1. make sure you have standard repo structure (check https://github.com/nirvdrum/svn2git if you have another strucutre)
2. have your authors file ready if needed
3. bundle install
4. svn2git <repo> --authors ~/authors.txt

standard repo strucutre
-----------------------

    trunk
      ...
    branches
      1.x
      2.x
    tags
      1.0.0
      1.0.1
      1.0.2
      1.1.0
      2.0.0


Quick steps
-----------

make sure you have git, ruby and rubygems installed

    $ sudo apt-get install git-svn
    $ git clone https://github.com/modsaid/using-svn2git.git
    $ cd using-svn2git
    $ bundle install
    $ mkdir ../new_repo && cd ../new_repo
    $ svn2git http://svn.example.com/path/to/repo --authors ~/authors.txt    

Credits
-------

Author: modsaid <mahmoud@modsaid.com>
Thanks to the svn2git original creators