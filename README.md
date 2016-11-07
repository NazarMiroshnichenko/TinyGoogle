# TinyGoogle

TinyGoogle built with Flask + Bootstrap + Google CSE

<p align="center">
  <a href="http://tinygoo.herokuapp.com/" target="\_blank">
    <img src="static/images/readme/demo.png" width="700px">
		<br>
    <h3>Live Demo</h3>
  </a>
</p>


## Features

* Search content by Google Custom Search API
* Ignore gfw to use google search

## Build Setup

1. install requirements
```bash
pip install -r requirements.txt
```
2. run
```bash
python app.py
# server at http://127.0.0.1:5000
```
or
```bash
gunicorn app:app  
# server at http://127.0.0.1:8000
```

## Config

1. in `data/engine.json`, you can change&add the engine's `key` and `cx` values:
```
  {
    "YOUR_ENGINE":{
      "name":"YOUR_NAME",
      "key":"YOUR_API_KEY",
      "cx":"YOUR_ENGINE_ID"
    }
  },
```
2. where to get CSE ID and Google API key :

  [Google CSE](https://cse.google.com/) & [Google API Console](https://console.developers.google.com/)

## Todo

* page-content-minigame(just like doodle)