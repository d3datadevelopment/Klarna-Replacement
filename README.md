# Klarna replacement if module is not used

This package removes the unused OXID Klarna module package from the shop and prevents conflicts in later updates.

## Install

if the Klarna module is not used and should be removed from the shop installation

* Deactivate the Klarna module in the shop backend.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    composer require d3/oxid-klarna-replacement --update-no-dev
    
* Manually remove the files from source/modules/tc/tcklarna.

## Uninstall

if the Klarna module is to be used again

* Manually clean up the replacement module entry (d3/oxide-klarna-replacement) from the vendor/composer/installed.json and composer.lock files.
* Run this composer statement in your shop. Adjust this instruction if your installation requires it.

    composer update --no-dev
