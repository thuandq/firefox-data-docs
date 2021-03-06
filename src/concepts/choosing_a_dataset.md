# Choosing a Desktop Product Dataset

This document will help you find the best data source for a given analysis.

This guide focuses on descriptive datasets and does not cover experimentation.
For example, this guide will help if you need to answer questions like:

- How many users do we have in Germany, how many crashes we see per day?
- How many users have a given addon installed?

If you're interested in figuring out whether there's a causal link between two events
take a look at our [tools for experimentation](../tools/experiments.md).

## Table of Contents

<!-- toc -->

# Raw Pings

{{#include ../datasets/ping_intro.md}}

# Main Ping Derived Datasets

The [main ping] contains most of the measurements used to track performance
and health of Firefox in the wild.
This ping includes histograms, scalars, and events.

This section describes the derived datasets we provide to make analyzing this data easier.

## `clients_daily`

{{#include ../datasets/batch_view/clients_daily/intro.md}}

## `clients_last_seen`

{{#include ../datasets/bigquery/clients_last_seen/intro.md}}

## `main_summary`

{{#include ../datasets/batch_view/main_summary/intro.md}}

## `first_shutdown_summary`

{{#include ../datasets/batch_view/first_shutdown_summary/intro.md}}

## `client_count_daily`

{{#include ../datasets/obsolete/client_count_daily/intro.md}}


# Other Datasets

{{#include ../datasets/other/socorro_crash/intro.md}}

[main ping]: https://firefox-source-docs.mozilla.org/toolkit/components/telemetry/telemetry/data/main-ping.html
[crash ping]: https://firefox-source-docs.mozilla.org/toolkit/components/telemetry/telemetry/data/crash-ping.html
