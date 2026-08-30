# Huisartsenpraktijk De Vaart — website

Jekyll site, gehost via GitHub Pages (`github-pages` gem).

## Lokaal draaien

Vereist Ruby 3.3 (dezelfde versie die GitHub Pages gebruikt). Op macOS:

```bash
brew install ruby@3.3
export PATH="/opt/homebrew/opt/ruby@3.3/bin:$PATH"   # per shell-sessie, of zet dit in ~/.zshrc

bundle install                    # gems worden in vendor/bundle geïnstalleerd (staat in .gitignore)
bundle exec jekyll serve          # → http://127.0.0.1:4000
```

Wijzigingen aan de markdown/html-bestanden worden automatisch herbouwd; enkel `_config.yml`
vereist een herstart van de server.

## Onderhoud

- Dependabot opent PR's voor gem-updates; mergen en daarna lokaal `bundle install` draaien.
- Handmatig alles bijwerken: `bundle update github-pages`.
- Kwetsbaarheden checken: `gem install bundler-audit && bundle-audit check --update`.

## Notes to self

Check regularly for updates of:

Source: http://html5boilerplate.com, versie 4.3.0
- normalize.css
- main.css

Header bar
Header background:
Color text (page: )
Button background: #1B6666
