# Optical Lever Sensitivity Calibration

## Description
This app is written in Python and uses Streamlit. It is used to calibrate the inverse optical lever sensitivity. The piezoscanner position is determined using the manufacturer calibration and the applied voltage. The photodetector vertical difference signal (V) is then plotted as a function of piezoscanner position. We make the assumption that when the cantilever presses down on a hard surface the slope of the cantilever tip position as a function of the piezoscanner position = 1 and calculate the sensitivity in nm/V. Select a linear region of the plot and press fit line to determine the sensitivity. The app is made to work with a standard output file from HEKA patchmaster but can be repurposed for other formats if needed. importantly the values are based on the calibration of our particular instrument so minor changes to the V2nm function will be necessary if you would like to use it based on your own system. Contact me if you have any questions I would be happy to help!

## Prerequisites

Before you begin make sure you have Python 3.7 or higher. It may work with other versions but I have not tested it.

## Installation

```
git clone https://github.com/neuro-myoung/invols.git
```

Create a local virtual environment, activate it, and install the requried packages using either

```
pip install -r requirements.txt 
```
or with pipenv
```
pipenv install
```

With the prerequisite packages installed from theappropriate environment run the following command and the app will open in your local host.

```
streamlit run invols.py
```

Alternatively, a web version of this app is available on Streamlit Sharing ![here](https://share.streamlit.io/neuro-myoung/invols/invols.py).
An example of a working data file is found in the examples folder.

## Demo

Just drag and drop your file of interest, sinput your fit region, and you're done!

![Demo GIF](/demo/demo.gif)


## Contributing
To contribute to **Invols**, follow these steps:

1. Fork this repository.
2. Create a branch: git checkout -b *branch_name*.
3. Make your changes and commit them: git commit -m '*commit_message*'
4. Push to the original branch: git push origin *project_name* *location*
5. Create a pull request.

Alternatively see the GitHub [documentation](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on creating a pull request.

## Contributors

[@neuro-myoung](https://github.com/neuro-myoung)

## Contact

If you want to contact me you can reach me at michael.young@duke.edu

## License
This project uses an [MIT License](https://opensource.org/licenses/MIT)