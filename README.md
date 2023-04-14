# Digital Biomarker Discovery Pipeline (DBDP)
#### An open-source software platform for the development of digital biomarkers using mHealth and wearables.
### Learn More at [DBDP.org](https://dbdp.org) 
#

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

The DBDP is created by the **BIG IDEAS Lab** at Duke University: http://dunn.pratt.duke.edu/
If you use the DBDP in your work, please cite the DBDP: dbdp.org, the following publication, and any references within the module you use.

> Bent, B., Wang, K., Grzesiak, E., Jiang, C., Qi, Y., Jiang, Y., Cho, P., Zingler, K., Ogbeide, F.I., Zhao, A., Runge, R., Sim, I., Dunn, J. (2020). The Digital Biomarker      Discovery Pipeline: An open source software platform for the development of digital biomarkers using mHealth and wearables data. Journal of Clinical and Translational Science, 1-28. doi:10.1017/cts.2020.511 ([Link to Open Access Article](https://www.cambridge.org/core/journals/journal-of-clinical-and-translational-science/article/digital-biomarker-discovery-pipeline-an-open-source-software-platform-for-the-development-of-digital-biomarkers-using-mhealth-and-wearables-data/A6696CEF138247077B470F4800090E63))

Digital biomarkers are digitally collected data that are transformed into indicators of health outcomes. The BIG IDEAS Lab is developing digital biomarkers for a range of diseases and conditions using a variety of sensors. 

We believe that not only data, but also computational pipelines and algorithms should operate by the **FAIR principles** (Findable, Accessible, Interoperable, and Reusable).

Digital biomarkers currently require extensive domain knowledge and computing skills. The purpose of the DBDP is to provide code sets, functions, and algorithms for the entire digital biomarker discovery pipeline to make discovering digital biomarkers more accessible. From the input of wearable sensor data to the development of machine learning and deep learning algorithms, we have provided an open source software resource for the digital biomarker community. 


### Instructions

For general help with the DBDP, see our [USER GUIDE](https://github.com/DigitalBiomarkerDiscoveryPipeline/DBDP/wiki/USER-GUIDE).
Please refer to specific DBDP modules for instructions for use. 

The [Digital Biomarker Discovery Resource Guide](https://github.com/DigitalBiomarkerDiscoveryPipeline/DBDP/wiki/Digital-Biomarker-Discovery-Resources) is available now!





### DBDP Modules

The results of this method on the following wearable sensors:

| Module | Pipeline | Wearables currently supported | Languages | Status |
| ------ | ------ | ------ | ------ | ------ | 
| Pre-processing | General | Basis Devices, Empatica E4, Garmin Vivosmart3, ECG, Non-specific | Python, R | Ongoing Development |
| Exploratory Data Analysis | General | Non-specific | Python, R | Ongoing Development |
| Glucose Variability |  | CGM (Dexcom), Support for other CGM | Python | Published package PyPi: cgmquantify |
| Resting Heart Rate |  | Fitbit, Non-specific | R | Published |
| Heart Rate Variability |  | Non-specific ECG, PPG | Python | Ongoing Development |
| Sleep |  | Garmin vivosmart 3 | Python | In Development |
| Mental Health |  | Actigraph, EEG | Python | In Development |
| Human Activity Recognition |  | Empatica E4, Non-specific | Python | Ongoing Development |




### Contributing

For inclusion into the digital biomarkers discovery pipeline, please follow the instructions in the Instructions subdirectory and create an Issue.
# Contribution guide

KerasNLP is an actively growing project and community! We would love for you
to get involved. Below are instructions for how to plug into KerasNLP
development.

## Background reading


## Contributing code

Before contributing code, please fill our form our [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe-hMOTwrSNaX0d7JyqhZP-6TrmRel9tXJLpclCP1tjGMWzgQ/viewform) and
[API Design Guide](API_DESIGN_GUIDE.md).

### Step 1. Open an issue

Before making any changes, we recommend opening an issue (if one doesn't already
exist) and discussing your proposed changes. This way, we can give you feedback
and validate the proposed changes.

If your code change involves the fixing of a bug, please include a
[Colab](https://colab.research.google.com/) notebook that shows
how to reproduce the broken behavior.

If the changes are minor (simple bug fix or documentation fix), then feel free
to open a PR without discussion.

### Step 2. Make code changes

To make code changes, you need to fork the repository. You will need to setup a
development environment and run the unit tests. This is covered in section
"Setup environment".

### Step 3. Create a pull request

Once the change is ready, open a pull request from your branch in your fork to
the master branch in 
[keras-team/keras-nlp](https://github.com/keras-team/keras-nlp).

### Step 4. Sign the Contributor License Agreement

After creating the pull request, you will need to sign the Google CLA agreement.
The agreement can be found at
[https://cla.developers.google.com/clas](https://cla.developers.google.com/clas).

### Step 5. Code review

CI tests will automatically be run directly on your pull request.  Their
status will be reported back via GitHub actions.

There may be several rounds of comments and code changes before the pull
request gets approved by the reviewer.

### Step 6. Merging

Once the pull request is approved, a team member will take care of merging.

## Setting up an Environment

Python 3.7 or later is required.

Setting up your KerasNLP development environment requires you to fork the
KerasNLP repository and clone it locally. With the
[GitHub CLI](https://github.com/cli/cli) installed, you can do this as follows:

```shell
gh repo fork keras-team/keras-nlp --clone --remote
cd keras-nlp
```

Next we must setup a python environment with the correct dependencies. We
recommend using `conda` to install tensorflow dependencies (such as CUDA), and
`pip` to install python packages from PyPI. The exact method will depend on your
OS.

**Note**: Please be careful not to use the `tensorflow` pre-packaged with conda,
which is incompatible with `tensorflow-text` on PyPi, and follow the
instructions below.

### Linux (recommended)

To setup a complete environment with TensorFlow, a local install of keras-nlp,
and all development tools, run the following or adapt it to suit your needs.

```shell
# Create and activate conda environment.
conda create -n keras-nlp python=3.9
conda activate keras-nlp

# The following can be omitted if GPU support is not required.
conda install -c conda-forge cudatoolkit-dev=11.2 cudnn=8.1.0
mkdir -p $CONDA_PREFIX/etc/conda/activate.d/
echo 'export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/' >> $CONDA_PREFIX/etc/conda/activate.d/env_vars.sh
echo 'export XLA_FLAGS=--xla_gpu_cuda_data_dir=$CONDA_PREFIX/' >> $CONDA_PREFIX/etc/conda/activate.d/env_vars.sh
source $CONDA_PREFIX/etc/conda/activate.d/env_vars.sh

# Install dependencies.
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install -e "."
```

### MacOS

⚠️⚠️⚠️ MacOS binaries are for the M1 architecture are not currently available from
official sources. You can try experimental development workflow leveraging the
[tensorflow metal plugin](https://developer.apple.com/metal/tensorflow-plugin/)
and a [community maintained build](https://github.com/sun1638650145/Libraries-and-Extensions-for-TensorFlow-for-Apple-Silicon)
of `tensorflow-text`. These binaries are not provided by Google, so proceed at
your own risk.

#### Experimental instructions for Arm (M1)

```shell
# Create and activate conda environment.
conda create -n keras-nlp python=3.9
conda activate keras-nlp

# Install dependencies.
conda install -c apple tensorflow-deps=2.9
python -m pip install --upgrade pip
python -m pip install -r requirements-macos-m1.txt
python -m pip install -e "."
```

#### Instructions for x86 (Intel)

```shell
# Create and activate conda environment.
conda create -n keras-nlp python=3.9
conda activate keras-nlp

# Install dependencies.
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install -e "."
```

### Windows

For the best experience developing on windows, please install
[WSL](https://learn.microsoft.com/en-us/windows/wsl/install), and proceed with
the linux installation instruction above.

To run the format and lint scripts, make sure you clone the repo with Linux
style line endings and change any line separator settings in your editor.
This is automatically done if you clone using git inside WSL.

Note that will not support Windows Shell/PowerShell for any scripts in this
repository.

## Testing changes

KerasNLP is tested using [PyTest](https://docs.pytest.org/en/6.2.x/).

### Run a test file

To run a test file, run `pytest path/to/file` from the root directory of the
repository.

### Run a single test case

To run a single test, you can use `-k=<your_regex>`
to use regular expression to match the test you want to run. For example, you
can use the following command to run all the tests in `import_test.py`
whose names contain `import`:

```shell
pytest keras_nlp/keras_nlp/integration_tests/import_test.py -k="import"
```

### Run the full test suite

You can run the default testing suite by simply invoking pytest:

```shell
pytest
```

We annotate tests that are slower or require a network connection as "large",
and by default `pytest` will skip these tests. We run large tests continuously
on GCP. You can specify these by running:

```shell
pytest --run_large
```

Finally, for tests that are very slow and resource intensive (e.g. downloading
a 5GB checkpoint), we use an "extra_large" annotation and do not run them
continuously at all. You can specify these by running:

```shell
pytest --run_extra_large
```

When running "extra_large" tests, we recommend also specify a specific test file
so you aren't waiting around forever!

## Formatting Code

We use `flake8`, `isort` and `black` for code formatting.  You can run
the following commands manually every time you want to format your code:

- Run `shell/format.sh` to format your code
- Run `shell/lint.sh` to check the result.

If after running these the CI flow is still failing, try updating `flake8`,
`isort` and `black`. This can be done by running `pip install --upgrade black`,
`pip install --upgrade flake8`, and `pip install --upgrade isort`.



License
----

Apache 2.0

***
Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.


[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
