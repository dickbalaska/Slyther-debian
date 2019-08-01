# Slyther-debian
Debian packaging for Slyther3

To build a slyther3 debian package

	cd someplace
	git clone https://github.com/dickbalaska/slyther.git
	git checkout slyther3
	git clone https://github.com/dickbalaska/slyther-debian.git
	git checkout slyther3
	mv slyther-debian slyther/debian
	cd slyther
	debuild

someplace will now contain the resultant .deb file.
