---
layout: project
title: NuvoEx - Forward Logistics
excerpt: Nuvo Logistics forayed into Forward logistics. The operational processes and the corresponding conceptualization of technical system.
category: Peppertap / NuvoEx
---
<h1 class="heading">Highlights</h1>
1. Ready for 1M/month orders
2. Launched in 30 cities, 1300 pin codes, covering 80% of e-commerce volume
3. Realtime operations visibility enabled in curbing the shipment lost rate to less than 0.06%
4. Integrated with 30 e-commerce clients

<h1 class="heading">Principles</h1>
1. Micro-interaction level visibility to operations team
2. No ad-hoc order status change requests
3. System to accommodate all the workflows and business logic
4. System should prompt users if they are doing manual errors
5. Developer friendly integration process for clients

The most critical aspect of such an elaborate system is to maintain a balance between rigidness and flexibility. As a principle, the system allows mechanisms to correct any human error which should be duly authorized by appropriate employee in the operations hierarchy.

<h1 class="heading">Monitoring</h1>
In addition, we built a monitoring tool, Fincher, on top of all the data we were capturing at all the touchpoints in the system. Underneath Fincher, we deployed an open source tool called [Redash](https://redash.io/){:target="_blank_"} to take care of our monitoring needs without investing too many resources. This enabled us to quickly set up SQL queries to visualize data. The quick turn around on analytics enables operations team to always stay on top of on ground operations. This unprecedented visibility enables curbing shipments losses to less than `0.05%`. The industry standard stands close to two digits.

<h1 class="heading">developer friendliness</h1>
1. Detailed API documentation
2. Interactive API explorer
3. UI based Callback/Push APIs configuration

<h1 class="heading">Financial Reconciliation</h1>
1. Cash on delivery adds an additional burden on logistics companies of handling cash. Our system gives realtime visibility to cash due at a delivery partner and cash to be deposited in a Client's account. This results in substantial improvement in operating cash reserves.
2. System is integrated with 3 largest banks in India which cover most of the geography. As soon as a delivery partner deposits cash in Nuvo's account, his liability is reduced by that much in the system on realtime basis.
3. The logistics business involves a lot of disputes (raised by clients, delivery partners etc). For this, I designed a sub-system by leveraging an open source ticketing tool, [Redmine](http://www.redmine.org/){:target="_blank_"}, to raise disputes. This enables finance team in managing liabilities of parties involved in disputed shipments. Which in turn benefits operating cash reserves.

> Fellini - Delivery Executive App

<div class="device-container">
  <div class="cd-iphone-6 cd-silver device android">
    <div class="cd-body">
      <div class="cd-sound"></div>
      <div class="cd-sleep"></div>
      <div class="cd-camera"></div>
      <div class="cd-ear"></div>
      <div class="cd-home"></div>
      <div class="cd-screen cd-transition-slider">
        <!-- img, iframe, content, etc. goes here -->
        <img src="/assets/img/nuvoex/fellini-home.png" alt="Fellini Home">
        <img src="/assets/img/nuvoex/fellini-accept.png" alt="Fellini Accept Shipments">
        <img src="/assets/img/nuvoex/fellini-home.png" alt="Fellini Home">
        <img src="/assets/img/nuvoex/fellini-deliver.png" alt="Fellini Deliver Shipments">
        <img src="/assets/img/nuvoex/fellini-shipment.png" alt="Fellini Shipment Details">
        <img src="/assets/img/nuvoex/fellini-status-change.png" alt="Fellini Mark Shipment Status">
      </div>
    </div>
  </div>
</div>

> Stanton - Client Order Management Portal

<div class="device-container">
  <div class="cd-mac cd-pro cd-fill-parent device">
    <div class="cd-top"></div>
    <div class="cd-bottom"></div>
    <div class="cd-camera"></div>
    <div class="cd-notch"></div>
    <div class="cd-screen cd-transition-slider">
      <!-- img, iframe, content, etc. goes here -->
      <img src="/assets/img/nuvoex/stanton-upload.png" alt="Stanton - Upload Orders via CSV">
      <img src="/assets/img/nuvoex/stanton-sidebar.png" alt="Stanton - Allowed Actions">
      <img src="/assets/img/nuvoex/stanton-actions.png" alt="Stanton - Reattempt Delivery or Initiate Return">
      <img src="/assets/img/nuvoex/stanton-detail.png" alt="Stanton - Order Detail">
    </div>
  </div>
</div>
<br/>
<br/>
<h1 class="heading">System Overview</h1>
The system comprises of 10 web & mobile apps and couple of background apps. Just to give the glimpse of depth and width of the system, please go through the graphic below.
<br/>
<br/>
<img class="image-fullwidth" src="/assets/img/nuvoex/nuvo-forward.png" alt="Nuvo Logistics Forward System"/>