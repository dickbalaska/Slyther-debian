# slyther-debian
Debian packaging for slyther2

To build a slyther2 debian package

	cd someplace
	git clone https://github.com/dickbalaska/slyther.git
	git clone https://github.com/dickbalaska/slyther-debian.git
	mv slyther-debian slyther/debian
	mv slyther slyther2
	cd slyther2
	git checkout slyther2
	cd debian
	git checkout slyther2
	cd ..
	debuild

someplace will now contain the resultant .deb file.

To push a new version to (launchpad)[https://launchpad.net/~dickbalaska/+archive/ubuntu/slyther]
dick replaces the final debuild step with two scripts:

	./debian/updateVersions <new.version.number>
	./debian/releaseSlyther2

