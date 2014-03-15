Simple scripts you can use for working with rails.

### Rebuilding

    bin/rebuild -h

    Usage: bin/rebuild [options]

    -f, --flags F        Flags for the rebuild script (by default all of them)
                         l - bundle exec rake log:clear
                         a - bundle exec rake assets:clean
                         i - [ -e public/system ] && rm -R public/system/*
                         d - bundle exec rake db:drop
                         c - bundle exec rake db:create
                         m - bundle exec rake db:migrate
                         s - bundle exec rake db:seed
                         p - RAILS_ENV=production bundle exec rake assets:precompile
                         j - [ -e bin/delayed_job ] && bin/delayed_job restart
                         Example: dcms

    -e, --except E       Except flags for the rebuild script
                         See documentation for --flags

### Updating

    bin/update -h

    Usage: bin/update [options]

    -f, --flags F        Flags for the update script (by default all of them)
                         l - bundle exec rake log:clear
                         a - bundle exec rake assets:clean
                         g - git pull
                         b - bundle install
                         m - bundle exec rake db:migrate
                         p - RAILS_ENV=production bundle exec rake assets:precompile
                         j - [ -e bin/delayed_job ] && bin/delayed_job restart
                         Example: gm

    -e, --except E       Except flags for the update script
                         See documentation for --flags

**Author (Speransky Danil):**
[Personal Page](http://dsperansky.info) |
[LinkedIn](http://ru.linkedin.com/in/speranskydanil/en) |
[GitHub](https://github.com/speranskydanil?tab=repositories) |
[StackOverflow](http://stackoverflow.com/users/1550807/speransky-danil)

