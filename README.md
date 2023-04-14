<h1 align="center">

  <br>
  <img src="./assets/envisedge-banner-dark.png#gh-light-mode-only" alt="DBDP"/ height="350" width="700">
  <img src="./assets/envisedge-banner-light.png#gh-dark-mode-only" alt=" DBDP"/ height="350" width="700">
  <br>
  Envision the Edge like never before...
  <br>

</h1>

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


EnvisEdge allows users to simulate an edge computing environment to test their ideas and models before putting them in place on the edge. It takes care of all the complex stuff such as diversity across operating systems, computation power and communication mediums, allowing you to focus on the idea rather than the setup.

EnvisEdge allows researchers, developers and data scientists to experiment and test their hypotheses, and produce production-ready code without having direct access to the edge devices. Creating a path for global research and growth in the domains of federated learning and edge computing.


## Key features :star2:  

1. Provides a platform for global or remote teams to run and test their systems/models prior to deployment.
2. Run, train and test FL algorithms and ML models.
3. Can setup environment of your choice with any arbitrary hardware constraints such as RAM, CPU and more.
4. Experience Edge on cloud and your devices.
<br>



# Repo Structure 🏢

 ```
NimbleEdge/EnvisEdge
├── CONTRIBUTING.md                         <-- Please go through the contributing guidelines before starting 🤓
├── README.md                               <-- You are here 📌
├── datasets                                <-- Sample datasets
├── docs                                    <-- Tutorials and walkthroughs 🧐
├── experiments                             <-- Recommendation models used by our services
└── fedrec                                  <-- Whole magic takes place here 😜
      ├── communication_interfaces              <-- Modules for communication interfaces eg. Kafka
      ├── data_models                           <-- All data modules that will be used for communication and thier serializers and  deserializers
      ├── modules                               <-- All the modules related to transformers, embeddings etc.
      ├── multiprocessing                       <-- Modules to run parallel worker jobs
      ├── optimization                          <-- Modules realted to torch optimizers and gradient decesnt etc.
      ├── python_executors                      <-- Contains worker modules eg. trainer and aggregator
      ├── serialization                         <-- serialization interfaces for data models
      ├── user_modules                          <-- Envis modules for wrapping toech modules for users.
      └── utilities                             <-- Helper modules
├── fl_strategies                           <-- Federated learning algorithms for our services.
├── notebooks                               <-- Jupyter Notebook examples
├── scala-core                              <-- Backbone of EnvisEdge
├── scripts                                 <-- bash scripts for creating and removing kafka topics.
└── tests                                   <-- tests
```

# Quickstart
Update the config files of the model (can be found [here](https://github.com/NimbleEdge/EnvisEdge/tree/main/configs)) you are going to use with logging directory:

```yml
log_dir:
  PATH: <path to your logging directory>
```

Download kafka from [Here](https://www.apache.org/dyn/closer.cgi?path=/kafka/3.1.0/kafka_2.13-3.1.0.tgz) 👈
and start the kafka server using the following commands

```bash
bin/zookeeper-server-start.sh config/zookeeper.properties
bin/kafka-server-start.sh config/server.properties
```
Create kafka topics for the job executor

```bash
cd scripts
$ bash add_topics.sh
Enter path to kafka Directory : <Enter the path to the kafka directory>
kafka url: <Enter the URL on which kafka is listening e.g if you are running it on localhost it would be 127.0.0.1>
Creating Topics...
```
## Installation
Install the dependencies using virtual environment
```bash
mkdir env
cd env
virtualenv envisedge
source envisedge/bin/activate
pip3 install -r requirements.txt
```

Download the federated dataset

```bash
$ bash download.sh -f
Enter global data path : <Enter the path you want your dataset to be saved>
Enter model : <Enter the config file of the model to update with the dataset path>
Downloading femnist dataset...
```

Run data preprocessing with [preprocess_data](preprocess_data.py) . Using this dataset, you will prepare a client_id mapping in the dataset that will be sent to Python workers for training the model.
```bash
python preprocess_data.py --config configs/regression.yml
```

To start the multiprocessing executor run the following command:

```bash
$ python executor.py --config configs/regression.yml
```
To see how traning is done run the following command:
```bash
$ python tests/integration_tests/integration_test.py --config configs/regression.yml
```
# Getting started
* [Tuitorials : to help you get started with understanding and implementing envisedge](https://github.com/NimbleEdge/EnvisEdge/tree/main/docs/source/tutorials).

# Resources
* [EnvisEdge.ai](https://docs.nimbleedge.ai/)
* [Introduction to Python](https://docs.python.org/3/tutorial/)
* [Introduction to python libraries]()
* [Introduction to Edge Computing](https://www.coursera.org/lecture/iot-wireless-cloud-computing/5-10-edge-computing-pOK8T)
* [NimbleEdge Blogs](https://blog.nimbleedge.ai/)
* [NimbleEdge Twitter](https://twitter.com/nimbleedgeinc?s=11&t=EAZr_ENlCYqBi6qxGz394w)
* [NimbleEdge Linkedin](https://www.linkedin.com/company/nimbleedge/)




# Start Contributing

1. Before you begin, please read our [CONTRIBUTOR'S](https://github.com/NimbleEdge/EnvisEdge/blob/main/CONTRIBUTING.md) GUIDELINES.
2. Introduce yourself in the #introduction channel on [Discord](https://nimbleedge.ai/discord) ( Most of the talks and discussions happen here.)
3. Look for an open issue that interests you such as [`good first issue`](https://github.com/NimbleEdge/EnvisEdge/labels/good%20first%20issue), [`python`](https://github.com/NimbleEdge/EnvisEdge/labels/python), [`scala`](https://github.com/NimbleEdge/EnvisEdge/labels/scala), [`documentation`](https://github.com/NimbleEdge/EnvisEdge/labels/documentation%20%F0%9F%93%83) and more. Liverage labels feature as shown below.
![Label wise issue search](https://github.com/shaistha24/EnvisEdge/blob/main/assets/issues.gif)
4. Star, [Fork](https://docs.github.com/en/enterprise-server@3.4/get-started/quickstart/fork-a-repo), and [Clone](https://docs.github.com/en/enterprise-server@3.4/get-started/quickstart/fork-a-repo#cloning-your-forked-repository) the repo.
5. Get down to business. Do your work.
6. Push to your fork.
7. Send a [PullRequest](https://docs.github.com/en/pull-requests) to NimbleEdge/EnvisEdge.</br>

This project follows the [all-contributors](https://github.com/NimbleEdge/EnvisEdge/blob/main/CONTRIBUTING.md) specification.Contributions of any kind are welcome!!

# FAQ and Other Questions
You can know more about Nimbleedge on the [about nimbleedge page](https://www.nimbleedge.ai/about-us).If you have question about the code or any general question about the repository or project, please head towards our [discord](https://nimbleedge.ai/discord).

# License
EnvisEdge has a [Apache License 2.0](https://github.com/NimbleEdge/EnvisEdge/blob/refactor-user-module/LICENSE)
