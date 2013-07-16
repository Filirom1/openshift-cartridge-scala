# OpenShift scala Cartridge

## Use it

In OpenShift, choose a downloaded cartridge, with the following URL : http://cartreflect-claytondev.rhcloud.com/reflect?github=Filirom1/openshift-cartridge-scala

On git push, `sbt compile` will be called, then the script `start.sh` at the root of your repo will be called.

Example of `start.sh` script:

    #!/bin/bash
    sbt run com.example.Boot.main

Make sure `start.sh` is an executable file: `chmod +x start.sh` 
    
This cartidge embed a [spray](https://github.com/spray/spray-template) example
