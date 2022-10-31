# Vayu Astra

[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Community](https://img.shields.io/badge/Join-Community-blue)](https://developer.ibm.com/callforcode/solutions/projects/get-started/) [![Website](https://img.shields.io/badge/View-Website-blue)](https://sample-project.s3-web.us-east.cloud-object-storage.appdomain.cloud/)

A basic GitHub repository example for new [Call for Code](https://developer.ibm.com/callforcode/) projects and those that join the Call for Code with The Linux Foundation deployment initiative. Not all sections or files are required. You can make this as simple or as in-depth as you need. And don't forget to [join the Call for Code community](https://developer.ibm.com/callforcode/solutions/projects/get-started/).

> If you're new to open source, please consider taking the [free "Introduction to Open Source" class](https://cognitiveclass.ai/courses/introduction-to-open-source).
> 
> [![Open Source Foundations](images/open-source-foundations.png)](https://cognitiveclass.ai/courses/introduction-to-open-source)

_Read this in other languages: [English](README.md), [한국어](./docs/README.ko.md), [português](./docs/README.pt_br.md), [中文](./docs/README.zh.md)._ 

## Contents

- [Submission or project name](#submission-or-project-name)
  - [Contents](#contents)
  - [Short description](#short-description)
    - [What's the problem?](#whats-the-problem)
    - [How can technology help?](#how-can-technology-help)
    - [The idea](#the-idea)
  - [Demo video](#demo-video)
  - [The architecture](#the-architecture)
  - [Long description](#long-description)
  - [Project roadmap](#project-roadmap)
  - [Getting started](#getting-started)
  - [Live demo](#live-demo)
  - [Built with](#built-with)
  - [Contributing](#contributing)
  - [Versioning](#versioning)
  - [Authors](#authors)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)

## Short description

### What's the problem?

Are you aware that Air Pollution is the cause of 6·5 million deaths each year globally? It attributes 11.65% death every year. It not only takes away people's life but also largely affects on the quality of living. 
Carbon emissions cause climate change by trapping heat, and impact public health adversely - inhalation of high concentrations of CO2 directly harms people's respiratory system, causing breathlessness, headache , chest pains and even cardiovascular diseases.


### How can technology help?

We want to combine technology + motive + idea to design a system for air quality monitoring and its communication about the degradation of air, which will tell us amount of CO2 in air, along with oxygen levels, thanks to  IBM IoT services, this platform helped us to make our task easier. Along with monitoring CO2 , Oxygen, and dangerous gases levels, Vayu Astra will help user in detecting carbon emission pollution hotspot and will alert user regarding by sending them notification......
Idea is to deploy large number of low cost device across geographic location to collect respective data, analyse it with help of cloud platform and send this data to user and respective authorities so they can take actions regarding it.

### The idea
1)Predicts amount of CO2 in air
As CO2 levels increases it will give notification to user
2)

3)when there's any poisonous gas present in surrounding it will alert user about it by sending notification. 
4) if government authorities are using vayu astra..on dashboard they can see respective data regarding CO2 oxygen levels and other harmful gases..if any particular area as soon as CO2 emissions will increase they give it information about it and it will become easier for them to recognise that area..and take respective strict actions to  factors which are contributing to it ..


## Demo video

[![Watch the video](https://raw.githubusercontent.com/Liquid-Prep/Liquid-Prep/main/images/readme/IBM-interview-video-image.png)](https://youtu.be/vOgCOoy_Bx0)

## The architecture

![Video transcription/translation app](https://developer.ibm.com/developer/tutorials/cfc-starter-kit-speech-to-text-app-example/images/cfc-covid19-remote-education-diagram-2.png)

1) Vayu Astra hardware consists of low power, internet enabled setup that monitors air parameters ( CO2, oxygen levels, humidity, poisonous gases, temperature altitude etc) and sends it to IBM  Watson lot platform via MQTT
2) The node RED backend IBM cloud collects these parameters via MQTT
3) Once evaluation is done it stores the data instance on cloud database and sends the air quality information to the IBM dashboard for visual indication
4) In case if there's increase amount of CO2, less oxygen levels in surroundings, or if any poisonous gas is present in surrounding the node red backend sends a text message to subscribed user and  they can see the data on respective dashboard
5) The node RED backend sets up a websocket service for data transmission to vayu astra dashboard
6) Vayu Astra dashboard then displays data in number, chart, maps, air quality estimation etc
7) In any case hardware disconnects from internet it is capable to approximately asses the air quality and display through 16x2 LCD indicator
8) In future we are planning to minimize current hardware setup into a dongle .


## Long description

[More detail is available here](./docs/DESCRIPTION.md)

## Project roadmap

The project currently does the following things.

- Feature 1
- Feature 2
- Feature 3

It's in a free tier IBM Cloud Kubernetes cluster. In the future we plan to run on Red Hat OpenShift, for example.

See below for our proposed schedule on next steps after Call for Code 2021 submission.

![Roadmap](./images/roadmap.jpg)

## Getting started

In this section you add the instructions to run your project on your local machine for development and testing purposes. You can also add instructions on how to deploy the project in production.

- [sample-react-app](./sample-react-app/)
- [sample-angular-app](./sample-angular-app/)
- [Explore other projects](https://github.com/upkarlidder/ibmhacks)

## Live demo

You can find a running system to test at [callforcode.mybluemix.net](http://callforcode.mybluemix.net/).

See the "long description" field in our submission (not in this repo) for the log-in credentials.

## Built with

- [IBM Cloudant](https://cloud.ibm.com/catalog?search=cloudant#search_results) - The NoSQL database used
- [IBM Cloud Functions](https://cloud.ibm.com/catalog?search=cloud%20functions#search_results) - The compute platform for handing logic
- [IBM API Connect](https://cloud.ibm.com/catalog?search=api%20connect#search_results) - The web framework used
- [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
- [Maven](https://maven.apache.org/) - Dependency management
- [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

<a href="https://github.com/Call-for-Code/Project-Sample/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=Call-for-Code/Project-Sample" />
</a>

- **Billie Thompson** - _Initial work_ - [PurpleBooth](https://github.com/PurpleBooth)

## License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
