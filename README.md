# XP to Fiat Discord bot script

## Usage

1. 依存Gemインストール

~~~sh
$ bundle install --path vendor/bundle
~~~

2. 動作させるにはTOKENとCLIENT_IDを下記で取得し設定する必要があります

https://discordapp.com/developers/applications/me 

xp_fiat.rbの先頭付近の以下の箇所の`TOKEN`と`CLIENT_ID`を取得した値に置き換えてください。

~~~ruby
bot = Discordrb::Commands::CommandBot.new token: TOKEN, client_id: CLIENT_ID, prefix:'?'
~~~

3. とりあえず起動

Gemの管理がBundler経由になったので、以下のように`bundle exec`を忘れずに

~~~sh
$ bundle exec xp_fiat.rb
~~~
