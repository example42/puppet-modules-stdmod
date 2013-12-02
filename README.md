# Example42 Puppet Modules 3.x : StdMod

Released under the terms of Apache2 licence.

Copyright Alessandro Franceschi / Lab42 (and specific commits authors)

Official website: [http://www.example42.com](http://www.example42.com)

Official Support forum: [Google Groups](https://groups.google.com/forum/#!forum/example42-puppet-modules)


This repository collects all the Version 3.x [Example42](http://www.example42.com) Puppet modules ("StdMod"), included here as **git submodules**.

The **official repository** of Example42 Puppet modules on [GitHub](http://github.com/example42/puppet-modules) currently contains NextGen (2.x) and StdMod (3.x) modules.
Old and new modules can cohexist on the same setup, but they have some different naming for parameters.

3.x modules do not use anymore the params_lookup function for each parameter.


## INSTALLATION AND UPDATES

From September 2013 most of the modules are published, and regularly updated, on the **Puppet Forge**.

Use the Puppet module tool to query and install Example42 modules:

        puppet module search example42

You can get the 3.x only module set with:

        git clone --recursive https://github.com/example42/puppet-modules-stdmod.git

To update your local copy with the upstream version:

        cd /etc/puppet/modules # Or the directory where's you local copy
        git pull origin master
        git submodule init
        git submodule update

If you want to force an update on each submodule, even if not tracked on the main repo:

        git submodule foreach git pull origin master

At times you may need to resync git modules urls. You can do that with:

        git submodule sync


You can test these modules on a safe environment using the [Example42 Puppet Playground](https://github.com/example42/puppet-playground). Check it out!

## IMPORTANT NOTICE

October 2013.

This modules set has to be considered **experimental** as the StdMod namong standards have not been defined completely.

Some of the modules present here have slightly different naming patterns that will be fixed when a first "major" version of the standard is defined.

Some of the solutions presented might not work yet correctly and have not been tested on production.




[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/example42/puppet-modules-stdmod/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

