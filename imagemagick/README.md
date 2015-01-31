Description
===========

Installs ImageMagick and optionally Rmagick (RubyGem).

Requirements
============

## Platform:

Tested on:

* Ubuntu (10.04)
* RHEL (6.1, 5.7)

Usage
=====

To install just ImageMagick,

  include_recipe "imagemagick"

In your own recipe/cookbook. To install the development libraries,

  include_recipe "imagemagick::devel"

To install the RubyGem rmagick,

  include_recipe "imagemagick::rmagick"

Which will install imagemagick, as well as the development libraries for imagemagick (so rmagick can be built).

Ensure that JSON properties are set based on the environement eg.

```
{
    "platform": "centos" // "redhat", "centos", "fedora", "debian", "ubuntu"
}
```