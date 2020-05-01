# HomeLight Ruby Style

HomeLight shared ruby style configs.

## Installation

Add this line to your application's Gemfile:

```ruby
group :development do
  gem "hl_ruby_style"
end
```

And then execute:

```bash
$ bundle install
```

## Usage

Create a `.rubocop.yml` with the following directives:

```yaml
inherit_gem:
  hl_ruby_style:
    - default.yml
```

Now, run:

```bash
$ bundle exec rubocop
```

No need to include rubocop directly application dependencies. Hl-ruby-style will include specific versions of `rubocop`, `rubocop-performance`, `rubocop-rails` and `rubocop-rspec` that is shared across projects.
