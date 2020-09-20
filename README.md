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
- ECTO::changeset::update_body남김,글자수제한검

## DEV 3 :: VIEW
- VIEW::FORM_COMPONENT::body블럭만남김

## DEV 4 :: VIEW :: 즉각적인 업데이트 가능해짐
- Twitter.Timeline::add_broadcast,subscribe_function
- TwitterWeb.PostLive.Index::add_handle_info_function

## DEV 5 :: Twitter.Timeline :: 리스트 역순배열
- Twitter.Timeline::update_list_posts_function