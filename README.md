# AGILE TIME KEEPER (ATK)

This project permits to display a time keeper companion that help you track time sequence in a meeting.

![ATK screen](images/atk_screenshot.png)

## Serve the pages

You have to serve the page using a HTTP Server.

* With [node.js](https://www.npmjs.com/package/http-server):

```bash
http-server
```

* With [python 2](https://docs.python.org/2/library/simplehttpserver.html):

```bash
python -m SimpleHTTPServer 8080
```

* With [python 3](https://docs.python.org/2/library/simplehttpserver.html):

```bash
python -m http.server 8080
```

and go on [localhost:8080](http://localhost:8080)

## Configuration

You can set your timer by modifying the `data.json` file

### Set the title of your meeting

modify the "title" property.

```json
"title": "My title"
```

### Add a sequence

Add an object in the sequences array.
A sequence must contains three properties (title, duration and color).

```json
"sequences": [
    {
        "title": "Introduction",
        "duration": 1,
        "color": "red",
        "extra": "my introduction extra content"
    }
]
```

* 1 = a minute
* 0.1 = 6 sec
* colors available = blue, red, yellow, purple, green
* extra = optional

## Demo

You can find the ATK demo [here](https://zolenas.github.io/agile-time-keeper/)

## Next steps

* Modify the progression timer to display time and not percent
* Add a settings page to manage the progress bar.

## Authors

### Development Lead

* [**Frédéric Faure**](mailto:frederik.faure@gmail.com)

### Co-Author

* [**Nicolas Rouvière**](mailto:zesk06@gmail.com)

## License

This project is under MIT license - see the [LICENSE](LICENSE.md) file for details.
