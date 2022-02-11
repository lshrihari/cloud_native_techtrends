# TechTrends project

TechTrends is a Flask / Python / SQLite web-based news sharing application. Objective of this project is to demonstrate cloud-native development fundamentals. Starter code for this project has been provided by Udacity at this [link](https://github.com/udacity/nd064_course_1/tree/main/project/techtrends). This project demonstrates the following; screenshots attached relate to the number ordering provided below -

1. Best practices in application development - maintaining `healthz` and `metrics` endpoints and providing a logging mechanism.

2. Application containerization using Docker

3. Establishing a CI pipeline for the application using Github Actions

4. Installing and bootstrapping a Kubernetes cluster; deploying the packaged application in the cluster

5. Templatizing multiple versions of the application, for a staging and production deployment, using Helm charts

6. Using ArgoCD to establish a GitOps based CD mechanism that uses the helm charts defined above, to deploy separate staging and production applications, currently (but not necessarily) in the same Kubernetes cluster.

All of this has been done in a `vagrant` and `VirtualBox` based OpenSuse Leap VM with static IP `192.168.56.0`
