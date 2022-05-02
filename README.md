# The Essential Guide for Election Security

## About the project

Doc explainer for those that stumble on the repo goes here

## Contributing

Before contributing to the EGES, please read the [style guide](STYLEGUIDE.md).

## Installation

### Prerequisites
The documentation is built with [Sphinx](https://www.sphinx-doc.org/en/master/). Use of [pipenv](https://pipenv.pypa.io/en/latest/) is optional, but encouraged for easier requirements management, built-in virtual environments, and local testing. See the pipenv documentation for installation options.

### Setup

Navigate to the project directory (assuming you're not already there) and install the required packages.

```sh
cd /path/to/Essential-Guide-to-Election-Security
```

#### Install packages using pipenv

This one line should install all the necessary requirements.

```sh
pipenv install
```

#### Install packages using pip

Using pip, you'll have to specify the requirements file that contains the list of required packages.

```sh
pip install -r requirements.txt
```

### Build the documentation

If this is the first time you're building the documentation&ndash;or if you've made changes to any of the files&ndash;do the following:

```sh
cd docs
```

#### Build (if pipenv)

```sh
pipenv run sphinx-build -b html source build
```

#### Build (if pip)

```sh
sphinx-build -b html source build
```

### View the documentation

After executing the above, navigate to the `docs` folder and run the following commands:

```sh
python -m http.server --directory build
```

Open a browser and connect to [http://localhost:8000](http://localhost:8000) and you should see the documentation.

### Keeping requirements up to date

Regardless of whether you're using either `pipenv` or `pip`, there are two requirements files to be kept up to date: the `Pipfile` and `requirements.txt`. `Pipenv` is useful for local development, but [Read the Docs](https://readthedocs.org/) will only install from `requirements.txt`. When you perform `pipenv install <some_package>`, `pipenv` updates the `Pipfile` for you. To update `requirements.txt`, run the following command:

```sh
pipenv run pip freeze > requirements.txt
```

This will overwrite the existing `requirements.txt` file with the newest updates.

If you add a package with `pip`, you'll have to edit the `Pipfile` with the package and version using the [required syntax](https://github.com/pypa/pipfile).
