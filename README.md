Instituto Superior Técnico, Universidade de Lisboa

**Network and Computer Security**

# Lab guide: ...
## Goals
The goal of this repository is to learn how to execute a collision attack on hash algorithm sha-1. You will learn how to use an Open-Source Python function on your local machine, you will also analyse the function step-by-step. We will use the function of the following public repository: 
https://github.com/nneonneo/sha1collider.

## Introduction

## Setup
Before starting this assignment you will need a few steps to be able to execute the attack:

- At first you will need to install python:

```bash
$ sudo apt-get install python3
```

- Then you will need to clone this repository into your workspace

```bash
$ git clone https://github.com/tecnico-sec/Fake-Signature-Attack.git
```
or via SSH

```bash
$ git clone git@github.com:tecnico-sec/Fake-Signature-Attack.git
```

- You need to install the library Pillow.

```bash
$ pip install Pillow
```

- You need to install ghostscript:
```bash
$ sudo apt-get update
$ sudo apt-get -y install ghostscript
```

- You need to install cjpeg:
```bash
$ sudo apt-get update
$ sudo apt-get -y install cjpeg:
```

You are now able to execute the attack:
Execute the following command:
```bash
$ python3 collide.py eve.pdf eve1B.pdf
```

Note that two new pdfs were generated, out-eve.pdf and out-eve1B.pdf.
Calculate the Sha1 hash code to both files.

```bash
$ sha1sum out-eve.pdf
$ sha1sum out-eve1B.pdf
```

Compare the two hashes.

**Acknowledgments**
...
----

[SIRS Faculty](mailto:meic-sirs@disciplinas.tecnico.ulisboa.pt)
