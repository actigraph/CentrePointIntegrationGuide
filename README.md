# ActiGraph's CentrePoint System Integration Guide

## Overview
This document contains an overview of the system integration options with ActiGraph’s [CentrePoint](https://actigraphcorp.com/centrepoint/) System

## CentrePoint Webhook System
An available option to have data *flowing* from the CentrePoint System into any external Electronic Data Capture (EDC) system is to utilize the [CentrePoint Webhook System](https://github.com/actigraph/CentrePointWebhookDocumentation). 

Webhooks allow you to build or set up integrations which subscribe to certain events on ActiGraph's CentrePoint ecosystem. When one of those events is triggered, CentrePoint will send a HTTP POST payload to the webhook's configured URL. 

With the Webhook architecture, CentrePoint will PUSH webhook events to clients containing specific metadata on the event which allow clients to then PULL in the related data. EDCs (and other clients) can utilze the CentrePoint APIs to retrieve new subject data as it becomes available (or is processed) in CentrePoint via a PULL service architecture. 


You can view the documentation for the CentrePoint Webhooks System [here](https://github.com/actigraph/CentrePointWebhookDocumentation). 


