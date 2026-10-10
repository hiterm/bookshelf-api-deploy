# bookshelf-deploy

Deployment configuration for Bookshelf.

API releases update a single deployment pull request from `deploy/bookshelf-api`
to `main`. While that pull request is open, subsequent releases replace its image
version and digest and update its title and description. After it is merged, the
next release creates a new pull request. Releases already deployed on `main` do
not create a pull request.
