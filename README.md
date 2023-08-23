# Awesome Rails Security
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of security resources for a Ruby on Rails application

## Table of Contents

- [Gems](#gems)
    - [Authentication and OAuth](#authentication-and-oauth)
    - [Authorization](#authorization)
    - [Rate Limiting](#rate-limiting)
    - [Request Management](#request-management)
    - [Static Code Analysis](#static-code-analysis)
    - [File Upload](#file-upload)
    - [Logging and Monitoring](#logging-and-monitoring0)
    - [Password Strength](#password-strength)
- [Tools](#tools)
    - [Static Code Analysis](#static-code-analysis)
    - [Logging and Monitoring](#logging-and-monitoring)
- [Security Vulnerability Advisory](#security-vulnerability-advisory)
- [Resources](#resources)
    - [Official Resources](#static-code-analysis)
    - [Labs - Vulnerable Applications](#labs-vulnerable-applications)
    - [Best Practices](#best-practices)
    - [Anti-Patterns](#anti-patterns)
    - [Additional Reading](#additional-reading)
- [Reporting Bugs](#reporting-bugs)

## Gems

### Authentication and OAuth
- [Devise](https://github.com/plataformatec/devise) - Flexible authentication solution for Rails with Warden
- [Devise Security](https://github.com/devise-security/devise-security) - A Devise extension to add additional security features required by modern web applications
- [Warden](https://github.com/wardencommunity/warden) - General Rack Authentication Framework
- [AuthLogic](https://github.com/binarylogic/authlogic) - An unobtrusive ruby authentication library based on ActiveRecord
- [OmniAuth](https://github.com/omniauth/omniauth) - A library that standardizes multi-provider authentication for web applications
- [JWT](https://github.com/jwt/ruby-jwt) - A ruby implementation of the RFC 7519 OAuth JSON Web Token (JWT) standard
- [Knock](https://github.com/nsarno/knock) - Seamless JWT authentication for Rails API

### Authorization
- [CanCanCan](https://github.com/CanCanCommunity/cancancan) - An authorization library for Ruby and Ruby on Rails which restricts what resources a given user is allowed to access.
- [Pundit](https://github.com/varvet/pundit) - Pundit provides a set of helpers which guide you in leveraging regular Ruby classes and object oriented design patterns to build a simple, robust and scaleable authorization system

### Rate Limiting
- [ReCaptcha](https://github.com/ambethia/recaptcha/) - A plugin that adds helpers for the reCAPTCHA API

### Request Management
- [Secure Headers](https://github.com/twitter/secure_headers) - Manages application of security headers with many safe defaults
- [Rack::Attack](https://github.com/kickstarter/rack-attack) - Rack middleware for blocking & throttling
- [ssrf_filter](https://github.com/arkadiyt/ssrf_filter) - A ruby gem for defending against Server Side Request Forgery (SSRF) attacks

### Static Code Analysis
- [Brakeman](https://github.com/presidentbeef/brakeman) - A static analysis security vulnerability scanner for Ruby on Rails applications
- [bundler-audit](https://github.com/rubysec/bundler-audit) - Patch-level verification for Bundler
- [Ruby Advisory Database](https://github.com/rubysec/ruby-advisory-db) - A database of vulnerable Ruby Gems. You can check your own Gemfile.locks against this database by using bundler-audit.
- [RoboCop](https://github.com/rubocop-hq/rubocop) - A Ruby static code analyzer and formatter, based on the community Ruby style guide
- [dawnscanner](https://github.com/thesp0nge/dawnscanner) - A source code scanner designed to review your ruby code for security issues

### File Upload
- [CarrierWave](https://github.com/carrierwaveuploader/carrierwave) - A gem that provides a simple and extremely flexible way to upload files from Ruby applications

### Logging and Monitoring
- [Exception Notification](https://github.com/smartinez87/exception_notification) - A gem that provides a set of notifiers for sending notifications when errors occur in a Rack/Rails application

### Password Strength
- [zxcvbn-ruby](https://github.com/envato/zxcvbn-ruby) - Ruby port of zxcvbn.js (Low-Budget Password Strength Estimation)

## Tools

### Static Code Analysis
- [rails_best_practices](https://github.com/flyerhzm/rails_best_practices) - A code metric tool to check the quality of Rails code
- [git-secrets](https://github.com/awslabs/git-secrets) - Prevents you from committing passwords and other sensitive information to a git repository
- [Snyk](https://snyk.io) - A developer-first solution that automates finding & fixing vulnerabilities in your dependencies
- [GuardRails](https://www.guardrails.io/) - Continuous security feedback for your GitHub repositories
- [Hakiri](https://hakiri.io/) - Hakiri monitors Ruby apps for dependency and code security vulnerabilities


### Logging and Monitoring
- [Sqreen](https://www.sqreen.com/) - Unified security monitoring and protection for modern cloud & on-prem environments
- [Report URI](https://report-uri.com/)

## Security Vulnerability Advisories
- [Ruby on Rails: Security](https://groups.google.com/forum/?fromgroups#!forum/rubyonrails-security) - A mailing list to get security announcements for Ruby, Rails, Rubygems, Bundler, and other Ruby ecosystem projects
- [ruby-security-ann](https://groups.google.com/forum/#!forum/ruby-security-ann) - Another mailing list to get security announcements for Ruby, Rails, Rubygems, Bundler, and other Ruby ecosystem projects
- [Ruby-Lang - Security](https://www.ruby-lang.org/en/security/) - A newsfeed for security vulnerabilities in the Ruby programming language
- [Synk - Vulnerability DB](https://snyk.io/vuln/?type=rubygems)


## Resources

### Official Resources
- [Rails - Securing Rails Applications](https://guides.rubyonrails.org/security.html) - This manual describes common security problems in web applications and how to avoid them with Rails


### Labs - Vulnerable Applications
- [OWASP RailsGoat](https://github.com/OWASP/railsgoat) - A vulnerable version of the Ruby on Rails Framework from versions 3 to 5. It includes vulnerabilities from the OWASP Top 10, as well as some "extras" that the initial project contributors felt worthwhile to share. This project is designed to educate both developers, as well as security professionals.
- [DeleteMe](https://github.com/rietta/DeleteMe) - Educational insecure Rails application
- [Checkmarx - Codebashing](https://free.codebashing.com/courses/ruby) - Lessons on common vulnerabilities implemented in Rails. Lessons on SQL Injection, XXE and Stored XSS are free.
- [PentesterLab](https://pentesterlab.com/exercises/) - Provides some vulnerable Rails environments to learn about security vulnerabilities, such as [CVE-2019-5420](https://pentesterlab.com/exercises/cve-2019-5420)

### Best Practices
- [rails-bestpractices.com](https://rails-bestpractices.com/) - A newsfeed of code snippets on what practices should and should not be done in Rails 
- [OWASP - Ruby on Rails Cheatsheet](https://github.com/OWASP/CheatSheetSeries/blob/master/cheatsheets/Ruby_on_Rails_Cheatsheet.md) - A cheatsheet that intends to provide quick basic Ruby on Rails security tips for developers. It complements, augments or emphasizes points brought up in the rails security guide from rails core
- [Preventing security issues in Ruby on Rails (based on OWASP cheatsheet)](https://medium.com/kkempin/preventing-security-issues-in-ruby-on-rails-based-on-owasp-cheatsheet-2fbca18b6a85)
- [OWASP - Ruby on Rails Security Guide](https://www.owasp.org/images/8/89/Rails_Security_2.pdf)
- [secure_rails](https://github.com/ankane/secure_rails)
- [Securing Sensitive Data in Rails](https://ankane.org/sensitive-data-rails)
- [production_rails](https://github.com/ankane/production_rails)
- [Rails Security Checklist](https://github.com/eliotsykes/rails-security-checklist)
- [Zen Rails Security Checklist
](https://github.com/brunofacca/zen-rails-security-checklist)
- [The Ruby Security Handbook](https://www.sqreen.com/checklists/ruby-security-handbook)
- [Ruby on Rails Security: Best Practices](https://www.codementor.io/ruby-on-rails/tutorial/ruby-on-rails-security-best-practices)
- [Ruby on Rails Security Basics](https://www.netsparker.com/blog/web-security/ruby-on-rails-security-basics/)
- [Ruby on Rails Security 17-Item Checklist](https://www.engineyard.com/blog/ruby-on-rails-security-checklist)
- [Level Up Your Security in Rails](https://blog.codeship.com/level-up-your-security-in-rails/)
- [Securing Ruby on Rails Web Applications](https://www.immun.io/hubfs/Immunio_2016/Content/Marketing/Securing_Ruby_on_Rails_Web_Applications_eBook.pdf)
- [Ruby on Rails Web Application Vulnerabilities: How to Make Your App Secure](https://rubygarage.org/blog/ruby-on-rails-web-application-vulnerabilities-how-to-make-your-app-secure)
- [Rails Security Strategy Book](https://bauland42.com/ruby-on-rails-security-strategy)
- [Preproduction Security Checklist for a Rails App](https://blog.codeship.com/preproduction-checklist-for-a-rails-app/)
- [Ruby on Rails Security Guide](https://sloboda-studio.com/blog/ruby-on-rails-security-guide/)

### Anti-Patterns
- [Rails' Insecure Defaults](https://codeclimate.com/blog/rails-insecure-defaults/)
- [The Inadequate Guide to Rails Security](https://www.honeybadger.io/blog/ruby-security-tutorial-and-rails-security-guide/)
- [Rails SQL Injection Examples](https://rails-sqli.org/)
- [Rails Vulnerabilities and Where to Find Them - Part 1](https://www.vdalabs.com/2018/01/12/rails-vulnerabilities-find-part-1/)
- [Rails Vulnerabilities and Where to Find Them - Part 2](https://www.vdalabs.com/2018/01/16/rails-vulnerabilities-find-part-2/)

### Additional Reading
- [Attacking Ruby on Rails Applications](http://www.phrack.org/issues/69/12.html#article)
- [The Evolution of Rails Security](https://speakerdeck.com/presidentbeef/the-evolution-of-rails-security)
- [Rails Security: above and beyond the defaults](https://www.randomerrata.com/articles/2017/rails-security/)
- [Fixing Command Injection Vulnerabilities in Ruby/Rails](http://gavinmiller.io/2015/fixing-command-injection-vulnerabilities/)
- [Fixing File Access Vulnerabilities in Ruby/Rails](http://gavinmiller.io/2015/fixing-file-access-vulnerabilities-in-ruby-and-rails/)
- [Fixing SQL Injection Vulnerabilities in Ruby/Rails](http://gavinmiller.io/2015/fixing-sql-injection-vulnerabilities/)

## Reporting Bugs
- [Ruby bug bounty program](https://hackerone.com/ruby)
- [Rails bug bounty program](https://hackerone.com/rails)
