**Note: project file should not be put inside virtual env file**
## create a envior, this where save in your current directory
`$ virtualenv [env name]`

## to activate env that you create
`$ source [env name]/bin/activate`

## list all packages installed to a txt, so other can use it
`$ pip freeze --local > requirement.txt`

## exit virtual env
`$ deactivate`

## delete a virtualenv
1. need to exit any virtual env
2. `$ rm -rf [env name]`

## install package with requirement.txt provided
`pip install -r requirement.txt`