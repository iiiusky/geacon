# Geacon

**Implement CobaltStrike's Beacon in Go**

----

*This project is only used for learning protocol analysis and reverse engineering. If someone's rights are violated, contact me to delete the project, and the last DO NOT USE IT ILLEGALLY*



## How to play

1. Setup the teamserver and start a http lisenter, the teamserver will generate the file `.cobaltstrike.beacon_keys`.
2. Compile beacontoo with Jetbrains Idea, use command `java -jar BeaconTool.jar ` to convert java keystore to PEM format.
3. Replace the RSA key pair in the file `cmd/config/config.go` (the RSA private key is not required, I wrote it in the code just for the record)
4. Compile geacon for what platform you want to run, use command `export GOOS="darwin" && export GOARCH="amd64" && go build cmd/main.go`
5. Having fun ! PR and issue is welcome ;)
6. Geacon has just been tested on CobaltStrike 3.14 and only support default c2profile, so many hardcode in the project and I will not try to implement more C2profile support at this moment.



## Protocol analysis

To be continued, I will update as soon as I have time ...

