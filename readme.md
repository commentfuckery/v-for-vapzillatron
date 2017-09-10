#Tooling
http://shopify.github.io/themekit/commands/

# Commands

## Upload

Upload will update all file states to Shopify and create any files that are not on Shopify’s servers. If upload is not provided with filename arguments it will do the whole project, otherwise you can upload individual files like this:

##### theme upload templates/404.liquid templates/article.liquid
Optional Flags

`--allenvs` : Will run this command for each environment in your config file.
Version

Version will print out the current version of the library.

## `Watch`

`theme watch -e ENV` <-- set in `config.yml` will start a process that will watch your directory for changes and upload them to Shopify. Any changes will be logged to the terminal and the status of the upload will be logged as well. The program can be stopped by simply typing ctrl+C.

To ease integrating the watcher with tools such as LiveReload, you can provide an the optional --notify argument with a file path that you want to have updated when the workers have gone idle. For example, if you had LiveReload watching for update made to a file at /tmp/theme.update you would enter the following command:

##### theme watch `--notify=/tmp/theme.update`
Optional Flags

`--allenvs` : Will run this command for each environment in your config file.
`--notify` : File path to a file that you want updated on idle.

## Client Side Notes:

1. When using the blog `gallery`, you must always have at least two images per post.  If you do not slider will be there with no images. The gallery was specifically contructed to be a gallery therefore if you wish to have further options, simply create another blog and post there.

<!-- TODO: FINISH DOCS -->

