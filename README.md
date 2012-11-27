# flask-authinator

A simple authentication web service, ready for deployment.


## Status

This project is currently in the works. Please don't use it for anything
production critical.


## What is This?

`flask-authinator` is a deployment-ready Flask web service that completely
manages user authentication for service oriented web applications.

The idea is that when building service oriented web applications, you ideally
want to separate out each part of your service (website, API, etc.) into
separate isolated components.

If I was building an API company, for instance, I'd create three separate
projects:

- mycompany-www (the user-facing website)
- mycompany-api (the developer-facing API)
- mycompany-accounts (the internal user accounts API and datastore)

Each of these projects would be hosted independently on their own servers. Each
of these projects would have their own database(s), their own cache(s), etc.

`flask-authinator` is a deploy-ready authentication service that:

- Uses PostgreSQL to store user data (email addresses, password hashes, etc.).
- Provides a REST API (with JSON responses) for your other service components to
  interact with (your website, your API, etc.).
- Allows you to create, edit, and remove users automatically.
- Runs on top of Heroku's cloud platform for instant scalability and ease of
  use.

If you need a simple way to manage users and user data in a distributed fashion,
look no further.
