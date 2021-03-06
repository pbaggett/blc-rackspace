# Broadleaf Commerce Community Module

[Check it out on GitHub](https://github.com/BroadleafCommerce/blc-rackspace)

## Rackspace

The broadleaf-rackspace module adds support for amazon functionality. Currently, this includes a Rackspace Cloud Files compatible `FileServiceProvider` implementation and registers that file provider as the default for the system.

The BroadleafFileService uses providers when working with files that are created by the system. This includes images and other media uploaded through the Broadleaf Admin as well as files generated by the system (e.g. site maps).

Distributed storage is required when running in a multi-server environment to ensure that images loaded on one server are available to the others in the cluster.  Other common alternatives are to use a shared drive via an NFS mount and configuring the `asset.server.file.system.path` property.

## Module Configuration
This module is compatible with BroadleafCommerce **3.1.0-GA**. Version 3.1.1-GA or later is recommended due to a  performance improvement that allows local caching of images stored on Cloud Files. To use the broadleaf-rackspace module requires that you  have a Rackspace account capabilities and some basic Broadleaf Commerce configuration.

For step-by-step instructions on how to integrate the amazon module into your project, see [[Module Installation]].
