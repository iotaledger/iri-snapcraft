
##First of all, install snapcraft

	sudo apt install snapcraft

##clone the project and in the directory run:

	snapcraft

##it will download all the dependencies and it will bundle a package called iri_1.1.0_{arch}.snap
##therefore run:

	sudo snap install iri_1.1.0_amd64.snap --force-dangerous

##and it will result in a 

	iri 1.1.0 installed

##then simply execute

	iri

The whole process should take around 2 minutes.



