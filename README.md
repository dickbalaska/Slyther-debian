# Slyther-debian
Debian packaging for Slyther

To build a slyther debian package
	cd someplace
	git clone https://github.com/dickbalaska/slyther.git
	git clone https://github.com/dickbalaska/slyther-debian.git
	mv slyther-debian slyther/debian
	cd slyther
	debuild

someplace will now contain the resultant .deb file.
