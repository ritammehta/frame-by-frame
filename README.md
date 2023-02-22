![FrameVis Banner](images/FrameVis_Banner.jpg)

FrameVis is a Python script for generating video frame visualizations, also known as "movie barcodes". These visualizations are composed of frames taken from a video file at a regular interval, resized, and then stacked together to show the compressed color palette of the video and how it changes over time.

## Installation

First, we're going to create a virtual environment to run this project. Start by installing virtualenvwrapper.
```shell
sudo pip3 install virtualenvwrapper
```

Then add the following 4 lines to your `~/.zshrc` file.
```shell
export WORKON_HOME=$HOME/.virtualenvs
export PROJECT_HOME=$HOME/Devel # This should be whatever your main projects folder is
source /usr/local/bin/virtualenvwrapper.sh
alias generate-color-timeline="python [path_to_this_folder]/frame-by-frame.py"
```
Reload the startup file:
`source ~/.bashrc`

Then create your virtualenv and install reqs while in this directory:
```shell
mkvirtualenv frame-by-frame
workon frame-by-frame
pip install -r requirements.txt
deactivate
```

## Run it
Just type
```shell
workon frame-by-frame
generate-color-timeline
```
into your terminal, and it should work!

## License

This script is licensed under the terms of the [MIT license](https://opensource.org/licenses/MIT). See the [LICENSE](LICENSE) file for more information.