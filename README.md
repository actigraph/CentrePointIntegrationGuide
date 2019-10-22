# ActiGraph's CentrePoint System Integration Guide

## Overview
This document contains an overview of the system integration options with ActiGraph’s [CentrePoint](https://actigraphcorp.com/centrepoint/) System

## CentrePoint Webhook System
An available option to have data *flowing* from the CentrePoint System into any external Electronic Data Capture (EDC) or other systems is to utilize the [CentrePoint Webhook System](https://github.com/actigraph/CentrePointWebhookDocumentation). 

Webhooks allow you to build or set up integrations which subscribe to certain events on ActiGraph's CentrePoint ecosystem. When one of those events is triggered, CentrePoint will send a HTTP POST payload to the webhook's configured URL. 

With the Webhook architecture, CentrePoint will PUSH webhook events to clients containing specific metadata on the event which allow clients to then PULL in the related data. EDCs (and other clients) can utilze the CentrePoint APIs to retrieve new subject data as it becomes available (or is processed). 


## CentrePoint APIs

#### CentrePoint V3 API

ActiGraph's has recently lauched the [CentrePoint V3 API](https://github.com/actigraph/CentrePoint3APIDocumentation) which provides additional flexibility to retrieve RAW sub-second resolution data.

The [CentrePoint V3 API](https://github.com/actigraph/CentrePoint3APIDocumentation) provides API endpoints for clients to retrieve RAW sub-second resolution actigraphy data between given time ranges which can be easily consumed and serialized. To view the supported formats/data definitions for retriiving RAW data in the [CentrePoint V3 API](https://github.com/actigraph/CentrePoint3APIDocumentation), view [RAW Data File Formats]( https://github.com/actigraph/CentrePoint3APIDocumentation/blob/master/sections/raw_data_file_formats.md).


The [CentrePoint V3 API](https://github.com/actigraph/CentrePoint3APIDocumentation) supports the following operations:

+ Adding/Editing Subjects
+ Assigning/Deploying ActiGraph Monitor to subject
+ Un-assigning ActiGraph Monitor from subject
+ Retrieve RAW sub-second subject data
+ Retrieve Epoch summary subject data
+ Retrieve general information on study/site configurations & subjects

#### CentrePoint V2 API



