source "https://rubygems.org"
gemspec

if ::File.directory?(gem_path = "../redis-store")
  gem "redis-store", "~> 1.1.0", path: gem_path
end

if ::File.directory?(gem_path = "../redis-rack")
  gem "redis-rack", "~> 1.5.0", path: gem_path
end

if ::File.directory?(gem_path = "../redis-activesupport")
  gem "redis-activesupport", '~> 4.0.0', path: gem_path
end

if ::File.directory?(gem_path = "../redis-actionpack")
  gem "redis-actionpack", "~> 4.0.0", path: gem_path
end

version = ENV["RAILS_VERSION"] || "4"

rails = case version
when "master"
  {:github => "rails/rails"}
else
  "~> #{version}.0"
end

gem "rails", rails
