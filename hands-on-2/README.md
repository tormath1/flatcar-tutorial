# Hands-on 2: provisioning

Hello, the goal here is to:
* provision a local Flatcar instance
* write Butane configuration
* generate the Ignition configuration
* boot the instance with the config

This is what we've done in the hands-1 but now it's done _as code_, we want to deploy an nginx container serving a "hello world" static webpage.

For this, there is an existing "config.yaml" (butane configuration), you need to write the content of /var/www/index.html (https://coreos.github.io/butane/examples/#files)

Hint: The Ignition configuration is a JSON file generated by Butane configuration. Butane (YAML) -> Ignition (JSON) -> Flatcar consumes this config.

# Resources

* https://coreos.github.io/butane/examples/
* https://coreos.github.io/ignition/rationale/
* https://www.flatcar.org/docs/latest/installing/#concepts-configuration-and-provisioning

# Demo

```
asciinema play demo.cast
```