# README

[Grow with Google - New England](https://github.com/growwithgooglema) collaborative project

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Description](#description)
- [Instructions](#instructions)
- [Repository contents](#repository-contents)
- [Running the application](#running-the-application)
  - [Docker](#docker)
  - [Local HTTP server](#local-http-server)
- [Contributors](#contributors)

## Description

- This is a progressive web application that uses Google Maps and MBTA APIs.
- We are developing on the `dev` branch.

## Instructions

- Please review the instructions in [CONTRIBUTING.md](CONTRIBUTING.md).
- Please behave according to the [Code of Conduct](CODE_OF_CONDUCT.md).

## Repository contents

- [data/](data): Code for gathering application data.
- [static/](static): CSS, image, and JavaScript files for the application.
  - [css/](static/css)
    - [custom.css](static/css/custom.css): Custom CSS for the app, in addition to Bootstrap.
  - [img/](static/img)
  - [js/](static/js)
    - [addratios.js](static/js/addratios.js)
    - [dbCaching.js](static/js/dbCaching.js)
    - [google-maps.js](static/js/google-maps.js)
    - [index.js](static/js/index.js)
    - [localforage.min.js](static/js/localforage.min.js)
    - [map.js](static/js/map.js)
    - [school.js](static/js/school.js)
    - [utilities.js](static/js/utilities.js): Calculates distances in order to display stop information based on the location searched.
    - [utilities.test.js](static/js/utilities.test.js)
- [.gitignore](.gitignore): List of instructions that tell Git to ignore certain files in the directory.
- [.jshintrc](.jshintrc)
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md): Guidelines for conduct.
- [CONTRIBUTING.md](CONTRIBUTING.md): Instructions for contributing to the repository.
- [Dockerfile](Dockerfile): Instructions for Docker container builds.
- [get_university_list.py](get_university_list.py):
- [index.html](index.html): The application homepage.
- [LICENSE](LICENSE): This file describes how the repository can be used by others. We have provided the repository under the MIT license, a permissive and widely-used license. See the [choose a license page](https://choosealicense.com/) for more info on licenses.
- [package-lock.json](package-lock.json):
- [package.json](package.json):
- [README.md](README.md): This file, a concise description of the repository.
- [sw.js](sw.js): This is the Service Worker file. Service Worker is a JavaScript file that sits between the browser and network requests. It helps to coordinate retrieval of information from the network and cache.
- [universities.html](universities.html): This is the webpage that shows the table with university accessibility data.
- [utilities.py](utilities.py): Python module with helper functions for the application. The functions calculate distances in order to display stop information based on the location searched.

## Running the application

### Docker

<!-- TODO: Update this section after setting up Docker

We have deployed our application to a [Docker](https://www.docker.com/) container.

The Docker container has been deployed to DockerHub.

The Docker container can also be run locally.

-->

### Local HTTP server

The main application resides inside the `index.html` file. To run it, you will need to start an HTTP server. `Python` offers a quick and dirty way to do this. Depending on whether you're on `python 2+` or `python 3+`, you should be able get an HTTP server started with the following:

*Note*: Please make sure you switch to the directory where the `index.html` file is.

In `python 2+`:

```bash
git clone git@github.com:growwithgooglema/gwg-mbta.git
cd gwg-mbta
python -m SimpleHTTPServer 8000
```

In `python 3+`

```bash
git clone git@github.com:growwithgooglema/gwg-mbta.git
cd gwg-mbta
python3 -m http.server 8000 -b localhost
```

If either of these two worked, head to [http://127.0.0.1:8000](http://127.0.0.1:8000) from your browser. The application is being served there.

*Note*: If you get any error related to a `PORT` issue, then it must be that you've got something running at port 8000; in which case, you should change 8000 to some other port that is not currently being used.

## Contributors

- [@AbdouSeck](https://github.com/AbdouSeck)
  - **Chief Data Wrangler**
  - **Friendly DevOps**
  - **Location Services**
- [@br3ndonland](https://github.com/br3ndonland)
  - **Nominated Benevolent Dictator**
  - **Dr. Documentation**
  - **Master of Markdown**
- [@jethridge13](https://github.com/jethridge13)
  - **Cartesian Contributor**
  - **Interstate Transportation Logistics**
- [@KonradSchieban](https://github.com/KonradSchieban)
  - **Cloudmaster**
  - **The Dockerizer**
- [@noirfatale](https://github.com/noirfatale)
  - **Front-End programming**
  - **Design Maven**
  - **People Ops**
- [@sereneliu](https://github.com/sereneliu)
  - **Front-End Ninja**