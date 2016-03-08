# django-setup-notes
Notes on using mod_wsgi Docker container to host Django
* Use the onbuild-tagged upstream container, otherwise things don't actually run
* The .whiskey directory is where the configuration actually takes place

# Build and run
docker build -t my-test-django .

docker run -dit -p 8000:80 --name test-django my-test-django

# Verify
http://[localhost]:8000


# Refs
* https://github.com/GrahamDumpleton/mod_wsgi-docker
* https://hub.docker.com/r/grahamdumpleton/mod-wsgi-docker/
* http://blog.dscpl.com.au/2014/12/hosting-python-wsgi-applications-using.html
