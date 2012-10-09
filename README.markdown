# Shopify Framework (WIP)
The minimium requirements for publishing a shopify theme.

## Setting up your local dev environment
Shopify doesn't have a "real" way to develop locally. However there is a Ruby Gem that will help you push changes to a Shopify test shop. Follow the steps below and you'll be able to push changes to Shopify from the command line.

1. Create a Test Shop in Shopify
2. Go to https://[your store].myshopify.com/admin/api and create a new private application.
3. Create a directory on you machine where you want to keep all the theme files
4. <code>cd</code> into that directory
5. <code>theme configure api_key password store_url</code>
6. <code>theme download</code> (Downloads the current theme into your folder)
7. From here you can edit your files and push them back to the server with theme upload <code>assets/layout.liquid</code> or <code>theme replace</code>. You could also use <code>theme watch</code> to push all updates the the server as soon as the file is changed.
8. Check the docs for additional commands or just type <code>theme help</code>.

(Thanks to Jeff Ammons for his post: http://jeffammons.net/2012/07/setting-up-a-development-environment-for-shopify-themes/)