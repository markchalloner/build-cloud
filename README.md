# Build::Cloud

Tools for building resources in AWS}

## Installation

Add this line to your application's Gemfile:

    gem 'build-cloud'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install build-cloud

## Usage

See the command line help for `build-cloud`.

## Changelog

2014-09-23 - version 0.0.6 - correctly name tags VPCs, and now allows you to refer to the public IP of a network interface (via `:network_interface_public_ip` in a Route 53 record set.

2014-09-16 - version 0.0.5 - now supports creation of DHCP Options Sets, and specifying them using the `:dhcp_options_set_name` key to a VPC.

2014-09-15 - version 0.0.4 - files can now be passed to `--config` with a path. It is no longer assumed that all files will be in the same directory.

2014-09-15 - version 0.0.3 - now accepts multiple files to `--config`. The second and subsequent files are merged into the first YAML file in order, ahead of any files specified in a `:include` list in the first YAML file.

2014-06-23 - version 0.0.2 - now accepts an array of files in the `:include` key in the given YAML config file. The files are merged in to the config file in the order that they are given.

2014-05-27 - version 0.0.1 - initial version.

## Contributing

1. Fork it ( http://github.com/<my-github-username>/build-cloud/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
