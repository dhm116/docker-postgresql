CenturyLink postgresql
=================

This image borrows heavily from [paintedfox/postgresql](https://registry.hub.docker.com/u/paintedfox/postgresql/). This image was created, however, to lock in the versions of the base image and postgresql to ensure it works in conjunction with other images and templates created with [Panamax](http://panamax.io).

Other changes include removal of `VOLUMES` from the dockerfile as these can be added later via a `docker run` or through Panamax.

Use the following environmental variables to create your database:

`DB` = Database name

`USER` = Database username

`PASS` = User's password

Example usage:
`docker run --name postgresql -e "DB=database1" -e "PASS=password" -e "USER=user1" centurylink/postgresql`

