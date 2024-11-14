[![Commit Activity](https://img.shields.io/github/commit-activity/m/Keffisor/jquery-spellchecker-lt)](https://github.com/Keffisor/jquery-spellchecker-lt/commits/master)
<br>
# jQuery-SpellChecker-LT
**jQuery-SpellChecker-LT** - Add a SpellChecker integration to any editor using LanguageTool's API.

## Demo
<img src="https://keffisor21.com/github/jquery-spellchecker-lt/imgs/preview.gif"/>
<img src="https://keffisor21.com/github/jquery-spellchecker-lt/imgs/1.png"/>
<img src="https://keffisor21.com/github/jquery-spellchecker-lt/imgs/2.png"/>
<img src="https://keffisor21.com/github/jquery-spellchecker-lt/imgs/3.png"/>
<p>You can try in the live demo at https://keffisor21.com/github/jquery-spellchecker-lt/.</p>

## Usage

You can just init the spellchecker with the default configuration using jQuery.
```js
$('#documentEditor').spellchecker();
```

### Custom Options

You can provide custom options to the spellchecker.
```js
$('#documentEditor').spellchecker({
  endpoint_url: "https://api.languagetool.org/v2/check",
  request_cooldown: 6.2
});
```

<b>Options available:</b>
- ```endpoint_url```: The URL where will connect to retrieve the spell check. This is ideal for set a custom languagetool server endpoint.
- ```request_cooldown```: Change the wait time when the user start's typing to connect into the endpoint.
- ```language```: Change the language of the spellchecker (default is "auto").
- ```username```: Your username/email as used to log in at languagetool.org for Premium API access.
- ```api_key```: Set to get Premium API access.