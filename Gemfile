# frozen_string_literal: true

source "https://rubygems.org"

# ========================
# Rails 基本
# ========================
gem "rails", "~> 8.0.2"
gem "puma", ">= 5.0"
gem "pg"                         # PostgreSQL
gem "sqlite3", ">= 2.1"          # SQLite（開発/テスト用途）

# ========================
# モダンアセット・JavaScript
# ========================
gem "propshaft"                 # モダンアセットパイプライン
gem "importmap-rails"          # ESMスタイルのJS読み込み
gem "turbo-rails"              # Hotwire: SPAライクな画面遷移
gem "stimulus-rails"           # Hotwire: JSフレームワーク
gem "tailwindcss-rails", "~> 4.3"

# ========================
# JSON API
# ========================
gem "jbuilder"

# ========================
# キャッシュ・ジョブ・WebSocket
# ========================
gem "solid_cache"
gem "solid_queue"
gem "solid_cable"

# ========================
# 本番環境用
# ========================
gem "kamal", require: false     # Dockerデプロイ
gem "thruster", require: false  # HTTP圧縮 & X-Sendfile

# ========================
# Windows用タイムゾーン
# ========================
gem "tzinfo-data", platforms: %i[windows jruby]

# ========================
# 起動高速化
# ========================
gem "bootsnap", require: false

# ========================
# 開発・テスト環境
# ========================
group :development, :test do
  # 環境変数 & 国際化
  gem "dotenv-rails"
  gem "rails-i18n"

  # デバッグ & コンソール
  gem "debug", platforms: %i[mri windows], require: "debug/prelude"
  gem "better_errors"
  gem "binding_of_caller"
  gem "pry-rails"
  gem "pry-byebug"
  gem "web-console"

  # 開発支援
  gem "bullet"                  # N+1検出
  gem "brakeman", require: false # セキュリティ静的解析
  gem "rubocop"                 # Rubyスタイルチェック
  gem "rubocop-rails"          # Rails向けルール
  gem "rubocop-rails-omakase", require: false

  # テスト系
  gem "rspec-rails"
  gem "factory_bot_rails"
  gem "faker"
end

# ========================
# その他のオプション
# ========================
# gem "bcrypt", "~> 3.1.7"      # 認証（has_secure_password使用時）
# gem "image_processing", "~> 1.2"  # ActiveStorageで画像変換を使う場合
