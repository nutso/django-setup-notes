# django-setup-notes
Notes on using mod_wsgi Docker container to host Django


Use the onbuild-tagged upstream container, otherwise things don't actually run


The .whiskey directory is where the configuration actually takes place



docker build -t my-test-django .

docker run -dit -p 8000:80 --name test-django my-test-django

http://<localhost>:8000
