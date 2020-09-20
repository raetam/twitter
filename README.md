# Twitter

To start your Phoenix server:

  * Install dependencies with `mix deps.get`
  * Create and migrate your database with `mix ecto.setup`
  * Install Node.js dependencies with `npm install` inside the `assets` directory
  * Start Phoenix endpoint with `mix phx.server`

# Dev log

## DEV 1
- mix phx.new twitter
- git init

## DEV 2 :: ECTO :: CREATE
- mix phx.gen.live Timeline Post posts username body likes_count:integer reposts_count:integer
- ECTO::schema::add_defaultvalue
- ECTO::changeset::add_post

## DEV 3 :: VIEW
- VIEW::FORM_COMPONENT::body블럭만남김