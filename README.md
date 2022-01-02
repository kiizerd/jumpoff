A simple starting point for Ruby on Rails 7 applications..  
Slight minimalized version of https://github.com/justalever/kickoff_tailwind

### Included gems

- [devise](https://github.com/plataformatec/devise)
- [friendly_id](https://github.com/norman/friendly_id)
- [sidekiq](https://github.com/mperham/sidekiq)
- [name_of_person](https://github.com/basecamp/name_of_person)

### Tailwind CSS by default

Includes setup for PostCSS to allow use of advanced TailwindCSS directives like `@layer` and `@apply`.  
Does this by adding `postcss-flexbugs-fixes postcss-import postcss-nested postcss-preset-env`  
npm packages a `postcss.config.js` configuration file, and a `--postcss` flag to the  
package.json build:css script

## How it works

When creating a new rails app simply pass the template filename and ruby extension through.

```bash
$ rails new sample_app -d <postgresql, mysql, sqlite3> -m template.rb
```

### Once installed what do I get?

- [Tailwind CSS](https://tailwind.com) by default. You may [opt for Bootstrap, Bulma, Sass, and PostCSS](https://github.com/rails/cssbundling-rails#installation) but this will require manual changes to the existing markup in the generated template view files.
- [Devise](https://github.com/plataformatec/devise) with a new `name` field already migrated in. The name field maps to the `first_name` and `last_name` fields in the database thanks to the [`name_of_person`](https://github.com/basecamp/name_of_person) gem.
- Enhanced views and devise views using Tailwind CSS.
- Support for Friendly IDs thanks to the handy [friendly_id](https://github.com/norman/friendly_id) gem. Note that you'll still need to do some work inside your models for this to work. This template installs the gem and runs the associated generator.
- Optional Foreman support. Run `.bin/dev` to kick off rails and Tailwind processes. Foreman needs to be installed as a global gem on your system for this to work. i.e. `gem install foreman`
- Custom view helper defaults for basic button and form elements.

### Boot it up

`$ ./bin/dev`

### Watch an overview

📹 Coming soon!

### Credits

Made by @justalever (yours truly). Find me on [Twitter](https://twitter.com/justalever), [web-crunch.com](https://web-crunch.com), [GitHub](https://github.com/justalever).
