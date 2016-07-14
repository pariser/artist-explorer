Name That Tune
==============

Forked from Artist Explorer -- fsahin/artist-explorer ([artistexplorer.spotify.com](https://artistexplorer.spotify.com/))

Name That Tune is a tool that helps you improve your "Name That Tune" skills.

The app pulls related artist information from Spotify and additional data (genre, biography) from the Echo Nest. Have a look at the documentation of these APIs at:

* [https://developer.spotify.com/web-api/](https://developer.spotify.com/web-api/)
* [https://developer.echonest.com/docs/v4](https://developer.echonest.com/docs/v4)

Running Locally
===============
**Not necessary but strongly suggested:** Create a [virtualenv] (http://docs.python-guide.org/en/latest/dev/virtualenvs/) or use an existing one before installing dependencies of this project.


Echo Nest API calls are proxied through a flask server. You need to start the server first.

```
cd server
pip install -r requirements.txt
python server.py
```

And you also need to serve the files at the root of the project. You can use SimpleHTTPServer module in python. To do that, change directyory to the project base and enter the following command:
```
python -m SimpleHTTPServer
```

App
===

Consumed Libraries:
--------------
* [d3](http://d3js.org/)
* [Google Gauge Charts](https://developers.google.com/chart/interactive/docs/gallery/gauge)
* [Spotify Web API Wrapper](https://github.com/JMPerez/spotify-web-api-js)
* [geoplugin](http://www.geoplugin.com/)
* [freegeoip](https://freegeoip.net)
