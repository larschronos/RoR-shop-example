ror shop
=================
Here I've done an example of shop which contains 2 pages:
- Main page (including live-loading of products);
- Cart page.

Also, I've done Admin's panel (based on ActiveAdmin) with permission through the /admin page (login: admin@example.com password: password).
You can add new products/categories/etc. there and so on and so forth.

I've implemented shopping cart using localStorage on client side.

Project based on [Mayak Rails website template](http://mayak.io).

You can check it out here: https://ror-shop-example.herokuapp.com/.

Getting Started
---------------

You can find required version of Ruby in file `.ruby-version` in the root directory of the application.

If you use RVM, add [.ruby-gemset file](http://stackoverflow.com/questions/15708916/use-rvmrc-or-ruby-version-file-to-set-a-project-gemset-with-rvm) to the root directory of the application.

Create file `config/database.yml` for database connection with content like:

    development:
      adapter: postgresql
      database: project_name
      pool: 5

There is `config/database_example.yml` for full example.

When done, run:

    $ bin/bundle install --without production
    $ bin/rake db:create db:migrate

You can install demo data using command: `bin/rake db:seed`

Application is ready to start. You can launch webserver `bin/rails server` and check home page at [localhost:3000](http://localhost:3000/) url.
