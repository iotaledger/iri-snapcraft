
# IOTA IRI SNAPCRAFT

## First of all, if you have Ubuntu install snapcraft

	$ sudo apt install snapcraft

## If you are not an Ubuntu user follow these instructions instead: http://snapcraft.io/docs/core/install

## clone the current project in a local directory and run:

	$ snapcraft

## Snapcraft will download all the dependencies and it will bundle a package called iri_1.1.0_{arch}.snap
## Therefore install snapd:

	$ sudo apt install snapd

# and run:

	$ sudo snap install iri_1.1.0_amd64.snap --force-dangerous

## and it will result in a '$ iri 1.1.0 installed'

## then simply execute

	$ iri ${PORT} ${NODES_LIST}

## for instance

	$ iri 14265 udp://1.1.1.1:142 udp://1.1.1.2:142 ...

The whole building process should take around 2 minutes.

# Know issues:

if you see this error message: 

	java.security.InvalidAlgorithmParameterException: the trustAnchors parameter must be non-empty

try running this:

	$ sudo apt-get install --reinstall ca-certificates-java
