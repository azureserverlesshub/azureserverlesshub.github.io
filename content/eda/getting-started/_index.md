---
weight: 1
description: Follow this guide to get started with Event Driven Architectures.
tags:
- getting-started
keywords:
- quickstart
type: "docs"
---
<!--more-->

## What are Event Driven Architectures ?
Event-driven architectures are a design paradigm that employs events and asynchronous communication to loosely couple an application’s components. These architectures can enhance agility and aid in the construction of reliable, scalable applications.

Serverless services such as Azure Event Grid, Azure Logic Apps,Azure Container Apps, Azure Service Bus, Azure Event Hubs, and Azure Functions align naturally with event-driven architectures - they are triggered by events, emit events, and possess inherent capabilities for building with events.

This guide introduces you with event-driven architectures. Comprehend the patterns within event-driven architectures and the Azure services that are frequently used to implement them. Learn best practices for constructing event-driven architectures, from designing event schemas to managing idempotency. Discover resources to get started with building event-driven architectures on Azure.

## What serverless services can you use to build event-driven architectures?

 
 {{<hextra/feature-grid cols="2" style="margin-top:10px">}}
  {{<feature-card-with-btn
    title="Azure Functions"
    subtitle="Azure Functions is a serverless solution that allows you to write less code, maintain less infrastructure, and save on costs. Instead of worrying about deploying and maintaining servers, the cloud infrastructure provides all the up-to-date resources needed to keep your applications running."
    icon="azure-function-apps"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/functions/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}

    {{<feature-card-with-btn
    title="Azure Logic Apps"
    subtitle="Azure Logic Apps is a cloud platform where you can create and run automated workflows with little to no code. By using the visual designer and selecting from prebuilt operations, you can quickly build a workflow that integrates and manages your apps, data, services, and systems."
    icon="azure-logic-apps"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/logic-apps/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}

  {{<feature-card-with-btn
    title="Azure Container Apps"
    subtitle="Azure Container Apps is a serverless platform that allows you to maintain less infrastructure and save costs while running containerized applications. Instead of worrying about server configuration, container orchestration, and deployment details, Container Apps provides all the up-to-date server resources required to keep your applications stable and secure."
    icon="azure-container-apps"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/container-apps/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}

    {{<feature-card-with-btn
    title="Azure Service Bus"
    subtitle="Azure Service Bus is a fully managed enterprise message broker, facilitates communication between applications and services. It achieves this by decoupling them, offering benefits such as load balancing work across competing workers, secure data routing across service & application boundaries, and reliable coordination for transactional work that requires a high-degree of reliability"
    icon="azure-service-bus"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/service-bus/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}
 
    {{<feature-card-with-btn
    title="Azure Event Grid"
    subtitle="Azure Event Grid is a highly scalable, fully managed Pub Sub message distribution service that offers flexible message consumption patterns using the MQTT and HTTP protocols. You can build data pipelines with device data, integrate applications, and build event-driven serverless architectures. It supports CloudEvents 1.0 specification to provide interoperability across systems."
    icon="azure-event-grid"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/event-grid/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}

    {{<feature-card-with-btn
    title="Azure Event Hubs"
    subtitle="Azure Event Hubs is a native data-streaming service in the cloud that can stream millions of events per second, with low latency, from any source to any destination. It also integrate seamlessly with other Azure services to unlock valuable insights. It is compatible with Apache Kafka and enables you to run existing Kafka workloads without any code changes."
    icon="azure-event-hub"
    firstBtnText="Patterns"
    firstBtnLink= "/patterns/"
    secondBtnText="Learn More"
    secondBtnLink= "https://azure.microsoft.com/en-us/products/event-hubs/"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.15),hsla(0,0%,100%,0));"
  >}}
  
  
  {{</hextra/feature-grid>}} 