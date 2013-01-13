SpreeEasyContact
================

Easy to implement contact form with honeypot-captcha, with a topic selection management in admin.
It stores all messages in DB for an easy recall of messages.

This extension is based on joshnuss spree-contact-form (thank you BTW) : https://github.com/joshnuss/spree-contact-form

Installation
============

Put the following line into your gemfile : 

gem 'spree_easy_contact'

Then run all the following command : 

bundle install

rake spree_easy_contact:install

rake db:migrate

Set properly the mail method in the admin area (/admin/mail_methods)

Add the following to your application initializers:

Spree::Config.set(:recaptcha_public_key => '[your_recaptcha_public_key]')
Spree::Config.set(:recaptcha_private_key => '[your_recaptcha_private_key]')

And you're done !
=================


Copyright (c) 2011 [Mathias Standaert for Organic Web], released under the New BSD License
