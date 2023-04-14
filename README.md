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
### Please see the DBDP/Instructions for a full and complete guide to contributing and for formatting.

#### Check out [GitHub's Guide to Contributing to Open Source Projects](https://opensource.guide/how-to-contribute/)

**Instructions for Adding to DBDP: **

If making a contribution to an existing repository:

1. Fork the existing repo
 ```python
https://github.com/DigitalBiomarkerDiscoveryPipeline/Digital_Health_Data_Repository
```

2. Clone forked repo locally
 ```python
git clone https://github.com/your_username/Digital_Health_Data_Repository
```
3. Make changes and commit/push to forked repo
4. Submit a pull request
5. Make an Issue in GitHub to let repo director (currently Brinnae) know so she can approve.

If making a contribution of a new repository:

1. Please contact the DBDP either by making a pull request in this [repo](https://github.com/DigitalBiomarkerDiscoveryPipeline/DBDP/) or contacting the Big Ideas Lab. We highly encourage contribution of new modules and would love to have you contribute! Every situation is different, but this is how it typically works:
- You become a member of the DBDP Organization
- You now have rights to make a new repo. If you want to retain the original repo in your own profile/organization we can just import the repo to the DBDP. If you want to transfer ownership of the repo, we can also make that happen. 

If you have questions, please reach out or submit an Issue in the corresponding DBDP module repository! 



## Background reading
Just getting started Please read through the [resources](https://github.com/DigitalBiomarkerDiscoveryPipeline/DBDP/wiki/Digital-Biomarker-Discovery-Resources)

## Contributing code

Before contributing code, please fill our form our [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSe-hMOTwrSNaX0d7JyqhZP-6TrmRel9tXJLpclCP1tjGMWzgQ/viewform) .

### Step 1. Open an issue

Before making any changes, we recommend opening an issue (if one doesn't already
exist) and discussing your proposed changes. This way, we can give you feedback
and validate the proposed changes.

### Step 2. Make code changes

To make code changes, you need to fork the repository. You will need to setup a
development environment.

### Step 3. Make the PR

To make code changes, you need to fork the repository. You will need to setup a
development environment.

## Contributors

Thank you to all of our wonderful [contributors](https://github.com/DigitalBiomarkerDiscoveryPipeline/Digital_Health_Data_Repository/graphs/contributors)


License
----

Apache 2.0

***
Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms.


