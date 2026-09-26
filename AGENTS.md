# Desk Ruby Client Instructions

`lib/desk/` implements Desk API resources and `spec/` contains RSpec fixtures and tests. Install with `bundle install`, then run `bundle exec rake spec` (the default Rake task also maps to `spec`) when the legacy Ruby dependencies work on the host.

Keep request paths, authentication, error translation, and fixture contracts aligned when changing a client method. Completion is the affected spec and Rake suite passing, or a precise dependency blocker. Never commit Desk credentials, customer/case payloads, or live API responses; use fixtures for local tests and report an authorized live API check separately.
