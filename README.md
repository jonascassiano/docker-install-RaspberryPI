# Raspberry PI docker Installation
 
For more thorough instructions for installing
on the supported distros, see the [install
instructions](https://docs.docker.com/engine/installation/).


## Installation:

From 'https://get.docker.com':
'''shell
curl -fsSL https://get.docker.com -o get-docker.sh
sh get-docker.sh
'''

## Setting up:

After installation, you need to add the 'pi' user to the 'docker' group:

'''shell
sudo usermod -aG docker pi
'''

After that, logout from your user:
'''shell
logout
'''

Once logged back in, you can use the command to check the user groups:
'''shell
groups
'''

## Testing:

To verify that the installation and configuration, you can run the following command:

```shell
docker run hello-world
```

## Legal
*Brought to you courtesy of our legal counsel. For more context,
please see the [NOTICE](NOTICE) document in this repo.*

Use and transfer of Docker may be subject to certain restrictions by the
United States and other governments.

It is your responsibility to ensure that your use and/or transfer does not
violate applicable laws.

For more information, please see https://www.bis.doc.gov

## Reporting security issues

The maintainers take security seriously. If you discover a security issue,
please bring it to their attention right away!

Please **DO NOT** file a public issue, instead send your report privately to
[security@docker.com](mailto:security@docker.com).

Security reports are greatly appreciated and we will publicly thank you for it.
We also like to send gifts—if you're into Docker schwag, make sure to let
us know. We currently do not offer a paid security bounty program, but are not
ruling it out in the future.

## Licensing

docker/docker-install is licensed under the Apache License, Version 2.0.
See [LICENSE](LICENSE) for the full license text.
