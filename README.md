# Openshift quickstart: Mezzanine on Django

This is a fork of [django-ex](https://github.com/openshift/django-ex) (please look there for global instructions) to deploy it on  [OpenShift](https://github.com/openshift/origin) cluster.

## Changes in this fork

* welcome - removed
* project/, manage.py - altered to fit provided by Mezzanine
* openshift/templates/ - renamed and altered
* requrements.txt - altered

## Howto add template to 'Create' page

1. upload mezzanine.json to master
2. run:

```bash
$ oc create -f mezzanine.json
```

## Hacks

For some not very much clean solutions i have to use to make some things working look to [mezzanine-ex-dirty](https://github.com/glowhost/mezzanine-ex).

## License

This code is dedicated to the public domain to the maximum extent permitted by applicable law, pursuant to [CC0](http://creativecommons.org/publicdomain/zero/1.0/).
