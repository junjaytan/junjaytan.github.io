---
layout: post
title: "Best Python Data Cleaning Libraries For People Data"
categories: data-analysis
---

In the past year I've had to do various projects that needed data clean up of typical contact info fields like emails and phone numbers. You'd think people would have solved these problems by now, and that have (kind of). If you use Python to do data cleaning, here are some libraries you will find useful:

### Validating Emails

Josh Tauberer, a known developer in the open government data movement, has developed an email validation library.

see: [https://github.com/JoshData/python-email-validator](https://github.com/JoshData/python-email-validator)

### Validating Phone Numbers

Google has a great Java-based library for parsing, formatting, storing, and validating international phone numbers. David Drysdale has converted this into a python version!

see: [https://pypi.python.org/pypi/phonenumbers](https://pypi.python.org/pypi/phonenumbers)

### Parsing Unstructured Addresses into Components

The Atlanta Journal Constitution in collaboration with DataMade, a "civic technology company," has released a python library for parsing unstructured USA address strings into address components. This library only parses addresses into components and does not validate that a given address is valid. But from deep firsthand experience having to use unstructured addresses, this alone is a powerful feature!

see: [https://github.com/datamade/usaddress](https://github.com/datamade/usaddress)

To validate that an address is valid, you will unfortunately most likely need to connect to some proprietary service like ArcGIS's API, Informatica Address Doctor, or Google Maps Enterprise. Alternatively, you might be able to connect to USPS's [address validation APIs](https://www.usps.com/business/web-tools-apis/address-information.htm) if you only have a small amount of addresses.

### Parsing Unstructured Names into Components

Instead of having to write your own name parser using Regular Expressions, you could use the nameparser library (early stage!).

See: [https://pypi.python.org/pypi/nameparser](https://pypi.python.org/pypi/nameparser)
