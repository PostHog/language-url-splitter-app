# language-url-splitter-app

With the deafult configuration, this app:

- Looks for a URL such as `/en` or `/en/anything`, where `en` is any lowercase two letter combination.
- Saves this string in an event property `locale`
- Updates the `$pathname` property and replaces `/en/bla` -> `/bla` inside it.   
- DOES NOT change the `$current_url` property