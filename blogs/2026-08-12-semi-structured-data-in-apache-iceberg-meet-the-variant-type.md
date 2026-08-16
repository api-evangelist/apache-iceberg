---
title: "Semi-Structured Data in Apache Iceberg: Meet the Variant Type"
url: "https://iceberg.apache.org/blog/variant-in-apache-iceberg/"
date: "2026-08-12"
author: "Neelesh Salian"
feed_url: "https://iceberg.apache.org/rss.xml"
---
Semi-structured data, such as JSON-like documents whose fields differ from row to row, has always been a poor fit for table formats built around fixed schemas. Iceberg v3 adds the Variant type for exactly this data: a single column can hold values of arbitrary, evolving shape, stored in a compact binary form that engines read and write consistently. This is the first post in a series on Variant in Apache Iceberg.
