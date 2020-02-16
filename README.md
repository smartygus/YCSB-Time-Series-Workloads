# YCSB Time Series Workloads

This is a collection of workload files that specify various workloads for used with the `TimeSeriesWorkload` class in YCSB.

They are designed to work with an expanded version of the `TimeSeriesWorkload` class that I developed, which is currenctly available in a fork [here](https://github.com/smartygus/YCSB/blob/cassandra-time-series/core/src/main/java/site/ycsb/workloads/TimeSeriesWorkload.java).

To use these workloads you will also need an adapter that implements the interface defined in the [`TimeseriesDB` class](https://github.com/smartygus/YCSB/blob/cassandra-time-series/core/src/main/java/site/ycsb/TimeseriesDB.java). I have implemented an adapter for Cassandra and ScyllaDB that can be found [here](https://github.com/smartygus/YCSB/tree/cassandra-time-series/cassandra-ts).

If you wanted to test these workloads on a Cassandra or ScyllaDB cluster of your own, you could simply build the `cassandra-ts` binding in my fork of YCSB, and use that directly.

If you wanted to setup a Cassandra or ScyllaDB cluster in Google Cloud for benchmarking purposes, I have also gathered a collection of utility scripts that may be useful [here](https://github.com/smartygus/gcloud-ycsb-ts-cassandra-scylla-utils).

Feel free to use, modify, or customise these workloads in anyway :)
