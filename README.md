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
- ECTO::changeset::update_remain only body

## DEV 3 :: VIEW :: FORM_COMPONENT
- VIEW::FORM_COMPONENT::update_remain only body

## DEV 4 :: VIEW :: new function become reactive
- Twitter.Timeline::add_broadcast,subscribe_function
- TwitterWeb.PostLive.Index::add_handle_info_function

## DEV 5 :: Twitter.Timeline :: list become inverse order
- Twitter.Timeline::update_list_posts_function

## DEV 6 :: VIEW :: EDIT function become reactive
- TwitterWeb.PostLive.Index::add_handle_info_function
- TwitterWeb.PostLive.Index::update_mount_function
- index.html::phx-update="prepend"