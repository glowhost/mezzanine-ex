# Openshift quickstart: Mezzanine on Django

This is a fork of [django-ex](https://github.com/openshift/django-ex) (please look there for global instructions) to deploy it on  [OpenShift](https://github.com/openshift/origin) cluster.

## Changes in this fork

* welcome - removed
* initial.json - added (see below about how to add)
* project/, manage.py - altered to fit provided by Mezzanine
* openshift/templates/ - renamed and altered
* requrements.txt - altered

## Adding initial pages

```bash
$ oc exec -p <name of pod> -- \ 
  env LD_LIBRARY_PATH=/opt/rh/python33/root/usr/lib64/ \
  PYTHONPATH=/opt/openshift/src/.local/lib/python3.3/site-packages \
  /opt/rh/python33/root/usr/bin/python3 manage.py loaddata initial
```

## License

This code is dedicated to the public domain to the maximum extent permitted by applicable law, pursuant to [CC0](http://creativecommons.org/publicdomain/zero/1.0/).
