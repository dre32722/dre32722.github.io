**Anki-MedRec Platform - Quickstart**
===================


# Medrec Microservices Documentation

This tutorial describes breaking down a monolithic application into a microservices architecture. We'll use the Avitek Medical Records as our monolithic application. 

## What is Medrec?

- End-to-end sample Java EE Application simulating a centralized medical record system
- Demonstrates various aspects of Java EE, WebLogic and its components
- Illustrates various design patterns
- [Avitek Medical Records Documentation](http://www.oracle.com/webfolder/technetwork/tutorials/obe/fmw/wls/12c/12_2_1/02-34-004-DeploySampleApplication/deploysampleapplication.html)


## Quickstart

1. Clone and run
```bash
$ git clone https://developer.em2.oraclecloud.com/developer49570-gse00010209/s/developer49570-gse00010209_medrec_4250/scm/medrec.git
$ cd medrec
$ git checkout dev
$ mvn -Pdev spring-boot:run
```

2. Access the Swagger page: [http://localhost:8080](http://localhost:8080)

<hr />
<a href="index" class="btn" >Go Back Home</a>
<hr />

