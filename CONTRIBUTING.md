## Fork, Clone, Setup
Fork the SpockBot repository, then clone your fork locally.

## Setup

### Configure remote
```
$ cd SpockBot
$ git remote add upstream git://github.com/SpockBotMC/SpockBot
```

### Install development dependencies
```
$ pip install -r dev-requirements.txt
```

### Install extra test interpreters
Installing the extra interpreters allows tox to test against multiple versions of python.
```
$ sudo apt-get install python27 python33 python34
```
## Development

### Create development branch
**Do not** work in the `master` branch, create a bug or feature branch and work from there.
`master` should always be a mirror of upstream master.
```
$ git checkout -b feature-tacocat
```
Please use a more descriptive branch name than `feature-tacocat`

### Hack away at the code
Have fun!

### Test your changes
Running `tox` will test that your changes pass all tests and follows the pep8 standard.
```
$ tox
```

### Pull Request
If `tox` comes back with a success you are ready for a pull request.
Commit your changes to your feature branch, push them to your fork and create a pull request.

## Testing
We highly encourage writing tests, we use the pytest framework and you can run `tox` to test your newly written tests.

