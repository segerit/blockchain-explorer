
<!-- (SPDX-License-Identifier: CC-BY-4.0) -->  <!-- Ensure there is a newline before, and after, this line -->

## Configure HTTPS to Hyperledger Explorer


#### Configure appconfig.json

- Edit file blockchain-explorer/appconfig.json
- Update config options
  - sslEnabled : true | false, to enable, or disable HTTPS.
  - sslCertsPath: "ssl-certs", by default it is in root of the project.
  - if sslEnabled is set to true, run $./keygenerator.sh to generate key, and certificate for HTTPS.

** NOTE:
  - The self-signed root certificate generated by ./keygenerator.sh script, has not been verified by a third party.
