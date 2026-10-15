# KhanAmaan55 Homebrew Tap

Homebrew formulae by [Amaan Khan](https://github.com/KhanAmaan55).

## DomainSpyder

Domain intelligence from one CLI: subdomain enumeration, DNS analysis, port
scanning, technology detection and WHOIS, with JSON and HTML reports.

```bash
brew install khanamaan55/tap/domainspyder
```

Works on macOS and Linux. Then:

```bash
domainspyder --help
brew upgrade domainspyder      # update to the latest release
brew uninstall domainspyder    # remove it
```

Or in a `brew bundle` `Brewfile`:

```ruby
tap "khanamaan55/tap"
brew "domainspyder"
```

Documentation, changelog and issues: <https://github.com/KhanAmaan55/DomainSpyder>

> Only scan domains and hosts you own or are authorised to test.

## Maintenance

New PyPI releases are picked up automatically. A daily workflow opens a
`domainspyder X.Y.Z` pull request about a day after each release, and
`brew test-bot` builds and tests it on macOS and Linux. Once it is green, run
**Actions → brew pr-pull** with the PR number to publish the bottles. Don't
merge these PRs with the Merge button.
