# google-analytics-standard-setup


Google Tag Manager

VARIABLES

Cross-Domain Tracking
Variable Type: Constant
Settings:
Value
comma-separated list of domains
Format Value
Change case to Lowercase

Click URL Hostname
Best for tracking external clicks.
Variable Type: Auto-Event Variable
Settings:
Variable Type
Element URL
Component Type
Host Name
strip 'www'
Format Value
Change case to Lowercase

TRIGGERS

Click - Outbound
Trigger Type: Click - Just Links
Settings:
Some Link Clicks
Click URL Hostname does not contain {Cross-Domain Tracking}


TAGS

Event - Click Outbound
Tag Type: Google Analytics - Universal Analytics
Track Type: Event
Category: conversion
Action: click outbound
Label: {{Click URL}}
Google Analytics Settings: {{Google Analytics Settings}}
Trigger: Click-Outbound



Google Analytics

Custom Dimensions
https://www.simoahava.com/analytics/13-useful-custom-dimensions-for-google-analytics/

1 Hit Timestamp     Hit
2 Session ID        Session
3 Client ID         User
4 User ID           User
5 Hit Type          Hit
6 Full Referrer     Hit
7 Payload Length    Hit
8 GTM Container ID  Hit
9 Redirect Count    Hit
10 Navigation Type  Hit
11 Tab Type         Hit
12 Tabs Open        Hit
13 Tab ID           Hit
14 Latitude         Session
15 Longitude        Session
