# The Essential Guide to Election Security

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

## Adding a new best practices

1. Create a dedicated issue for the new bp
1. Draft and finalize bp
1. Rebase if necessary
1. Add to index.rst
1. Add to bp_index.rst with priorities for each maturity
1. Update glossary and acronyms, if necessary
1. Check whether it needs to be added to maturity priorities
1. Squash and Merge PR into a staging branch (gets rid of nit pick commits)

## Publishing a new version

1. Create a dedicated branch off main, ideally named staging-202xqy or 20xqy-release. The date should be the quarter beginning when the version is released (e.g., q4 for the sep 30/oct 1 release)
1. Use issues/branches for all changes, then merge into staging branch
1. Update conf.py by incrementing version and release
1. Commit directly to staging-202xqy
1. Create and review PR for prepared staging branch into main
1. Merge commit into main (do not squash)
1. After merging, go to releases and select draft a new release
1. Title the release 202xqy release and create a tag called vx.x.x as appropriate
1. Provide a description, ideally including details of changes
