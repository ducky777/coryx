# Coryx

This documentation is meant for Alpha testers of Coryx.ai

# Installation
`pip install -i https://test.pypi.org/simple/ coryx`

# Set-up
Run `coryx init` and you will be prompted for your credentials. This will generate a `.coryxenv` file to store your credentials. 

**NOTE: THIS FILE NEEDS TO BE AT THE ROOT OF WHERE YOU ARE RUNNING CORYX**

# Quick start 
`git clone https://github.com/ducky777/coryx.git`

`coryx run -f {path_to_your_file.py} -o {path_to_output_directory}`

With `example_script.py` provided here, you can run

`coryx run -f example_script.py -o output -d -t`

## Arguments
### positional arguments:
  1. `run`: to run coryx to refactor
  2. `init`: to run for initial setup

### flags

`-f, --file`: **(REQUIRED)** path to your file to refactor.

`-o, --output`: Directory to save your refactored file. Defaults `./coryx_outputs`

`-t, --tests`: Set to enable test template generation based on refactored file

`-d, --docstring`: Set to enable auto docstring generation for refactored functions/methods.

# FAQs
## I am getting JSON decode error
Make sure your script does not have non ascii characters like Chinese characters or emojis.

## Dependencies are not installed properly when I pip install
If pip did not install the dependencies properly, manually install:
```sh
pip install requests
pip install python-dotenv
```

# Support
Join our slack channel for community support. Alternatively you can email us at tech@coryx.ai.
