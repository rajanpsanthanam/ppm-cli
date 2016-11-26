# ppm-cli
python package manager - command line interface

This script helps in managing the python dependecies in a single file. No need for maintaining dependecies across
multiple files per environment

below json structure depicts the dependecies for all the environment.

<pre><code>
{
  "dependencies": {
    "common": {
      "django": "1.10",
      "djangorestframework": "3.3.2"
    },
    "development": {
      "ipdb" : "\*"
    },
    "testing": {
      "pytest": "2.8.7",
      "pytest-django": "2.9.1"
    },
    "production": {
      "requests": "2.10.0"
    }
  }
}
</code></pre>

Note :
1. common denotes dependecies needed across all the environment
2. where * denotes the latest stable version available

add package.json to the root directory of the project and run packages script with one of the below actions.
project's virtualenv should be active while running the script

1. commands
2. unpack
3. difference
