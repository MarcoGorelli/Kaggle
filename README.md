

Select Python Interpreter
-------------------------

ctrl + shift + p -> select interpreter -> enter interpreter path -> find -> /opt/conda/bin/python

Extensions
----------

Install and enable [PyLance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance).

Kaggle API key
--------------

Follow instructions [here](https://www.kaggle.com/docs/api#getting-started-installation-&-authentication) to get an API key.
Temporarily save your `kaggle.json` file to this repository.

Set up development environment
------------------------------

Open this repository in vs code - see [here](https://code.visualstudio.com/docs/remote/containers) for instructions for developing
inside a container.

Move Kaggle API key
-------------------

From within the container in vscode run

```
mkdir /root/.kaggle
mv kaggle.json /root/.kaggle/
```

Verify it works by running:
```
kaggle competitions list
```

New competition
---------------

Make a new repository for it on GitHub. Then, for each new competition, do e.g.

```
git submodule add git@github.com:MarcoGorelli/tweet-sentiment-extraction.git
```

Any input for the competition goes in the `input` folder here.
