# PySpark Stubs

A collection of the Apache Spark [stub files](https://www.python.org/dev/peps/pep-0484/#stub-files). These files were generated by [stubgen](https://github.com/python/mypy/blob/master/mypy/stubgen.py) and manually edited to include accurate type hints.

Tests and configuration files have been originally contributed to the [Typeshed project](https://github.com/python/typeshed/). Please refer to its [contributors list](https://github.com/python/typeshed/graphs/contributors) and [license](https://github.com/python/typeshed/blob/master/LICENSE) for details.


## Usage

According to [PEP 484](https://www.python.org/dev/peps/pep-0484/#storing-and-distributing-stub-files): 

> Third-party stub packages can use any location for stub storage. Type checkers should search for them using PYTHONPATH. 

Moreover:

> Third-party stub packages can use any location for stub storage. Type checkers should search for them using PYTHONPATH. A default fallback directory that is always checked is shared/typehints/python3.5/ (or 3.6, etc.)

Adding `third_party/3` to the `PYTHONPATH` seems to the trick.

## API Coverage

| Module                                             | Dynamically typed | Statically typed | Notes            |
|----------------------------------------------------|-------------------|------------------|------------------|
| <s>pyspark.shell</s>                               | ✘                 | ✘                | Internal         |
| pyspark.rddsampler                                 | ✔                 | ✘                |                  |
| <s>pyspark.java\_gateway</s>                       | ✘                 | ✘                | Internal         |
| <s>pyspark.tests</s>                               | ✘                 | ✘                | Tests            |
| pyspark.join                                       | ✔                 | ✘                |                  |
| pyspark.statcounter                                | ✔                 | ✘                |                  |
| pyspark.serializers                                | ✔                 | ✘                |                  |
| <s>pyspark.heapq3</s>                              | ✘                 | ✘                | Internal         |
| pyspark                                            | ✔                 | ✘                |                  |
| <s>pyspark.traceback\_utils</s>                    | ✘                 | ✘                | Internal         |
| pyspark.profiler                                   | ✔                 | ✘                |                  |
| pyspark.storagelevel                               | ✔                 | ✘                |                  |
| pyspark.broadcast                                  | ✔                 | ✔                | Mixed            |
| <s>pyspark.worker</s>                              | ✘                 | ✘                | Internal         |
| <s>pyspark.shuffle</s>                             | ✘                 | ✘                | Internal         |
| pyspark.files                                      | ✘                 | ✔                |                  |
| <s>pyspark.find\_spark\_home</s>                   | ✘                 | ✘                | Internal         |
| pyspark.status                                     | ✔                 | ✘                |                  |
| <s>pyspark.daemon</s>                              | ✘                 | ✘                | Internal         |
| pyspark.context                                    | ✘                 | ✔                |                  |
| <s>pyspark.cloudpickle</s>                         | ✘                 | ✘                | Internal         |
| pyspark.accumulators                               | ✔                 | ✘                |                  |
| pyspark.version                                    | ✘                 | ✔                |                  |
| pyspark.resultiterable                             | ✔                 | ✘                |                  |
| pyspark.conf                                       | ✔                 | ✘                |                  |
| pyspark.rdd                                        | ✘                 | ✔                |                  |
| pyspark.ml.tuning                                  | ✘                 | ✘                |                  |
| pyspark.ml.clustering                              | ✘                 | ✘                |                  |
| pyspark.ml.feature                                 | ✘                 | ✘                |                  |
| <s>pyspark.ml.tests</s>                            | ✘                 | ✘                | Tests            |
| pyspark.ml.common                                  | ✘                 | ✘                |                  |
| pyspark.ml                                         | ✘                 | ✘                |                  |
| pyspark.ml.wrapper                                 | ✘                 | ✘                |                  |
| pyspark.ml.classification                          | ✘                 | ✘                |                  |
| pyspark.ml.recommendation                          | ✘                 | ✘                |                  |
| pyspark.ml.base                                    | ✘                 | ✘                |                  |
| pyspark.ml.regression                              | ✘                 | ✘                |                  |
| pyspark.ml.pipeline                                | ✘                 | ✘                |                  |
| pyspark.ml.util                                    | ✘                 | ✘                |                  |
| pyspark.ml.evaluation                              | ✘                 | ✘                |                  |
| <s>pyspark.ml.param._shared_params\_code\_gen</s>  | ✘                 | ✘                | Internal         |
| pyspark.ml.param                                   | ✘                 | ✘                |                  |
| pyspark.ml.param.shared                            | ✘                 | ✘                |                  |
| pyspark.ml.linalg                                  | ✘                 | ✘                |                  |
| pyspark.mllib.clustering                           | ✘                 | ✘                |                  |
| pyspark.mllib.feature                              | ✘                 | ✘                |                  |
| pyspark.mllib.tests                                | ✘                 | ✘                |                  |
| pyspark.mllib.common                               | ✘                 | ✘                |                  |
| pyspark.mllib.tree                                 | ✘                 | ✘                |                  |
| pyspark.mllib                                      | ✘                 | ✘                |                  |
| pyspark.mllib.classification                       | ✘                 | ✘                |                  |
| pyspark.mllib.recommendation                       | ✘                 | ✘                |                  |
| pyspark.mllib.regression                           | ✘                 | ✘                |                  |
| pyspark.mllib.util                                 | ✘                 | ✘                |                  |
| pyspark.mllib.evaluation                           | ✘                 | ✘                |                  |
| pyspark.mllib.random                               | ✘                 | ✘                |                  |
| pyspark.mllib.fpm                                  | ✘                 | ✘                |                  |
| pyspark.mllib.linalg.distributed                   | ✘                 | ✘                |                  |
| pyspark.mllib.linalg                               | ✘                 | ✘                |                  |
| pyspark.mllib.stat._statistics                     | ✘                 | ✘                |                  |
| <s>pyspark.mllib.stat.test</s>                     | ✘                 | ✘                | Tests            |
| pyspark.mllib.stat.distribution                    | ✘                 | ✘                |                  |
| pyspark.mllib.stat.KernelDensity                   | ✘                 | ✘                |                  |
| pyspark.mllib.stat                                 | ✘                 | ✘                |                  |
| pyspark.streaming.kafka                            | ✘                 | ✘                |                  |
| pyspark.streaming.flume                            | ✘                 | ✘                |                  |
| <s>pyspark.streaming.tests</s>                     | ✘                 | ✘                | Tests            |
| pyspark.streaming                                  | ✘                 | ✘                |                  |
| pyspark.streaming.listener                         | ✘                 | ✘                |                  |
| pyspark.streaming.util                             | ✘                 | ✘                |                  |
| pyspark.streaming.dstream                          | ✘                 | ✘                |                  |
| pyspark.streaming.context                          | ✘                 | ✘                |                  |
| pyspark.streaming.kinesis                          | ✘                 | ✘                |                  |
| pyspark.sql.types                                  | ✔                 | ✘                |                  |
| pyspark.sql.functions                              | ✘                 | ✔                |                  |
| pyspark.sql.catalog                                | ✘                 | ✔                |                  |
| <s>pyspark.sql.tests</s>                           | ✘                 | ✘                | Tests            |
| pyspark.sql.streaming                              | ✔                 | ✘                |                  |
| pyspark.sql.column                                 | ✘                 | ✔                |                  |
| pyspark.sql                                        | ✔                 | ✘                |                  |
| pyspark.sql.window                                 | ✔                 | ✘                |                  |
| pyspark.sql.session                                | ✔                 | ✘                |                  |
| pyspark.sql.utils                                  | ✔                 | ✘                |                  |
| pyspark.sql.group                                  | ✘                 | ✔                |                  |
| pyspark.sql.readwriter                             | ✔                 | ✘                |                  |
| pyspark.sql.dataframe                              | ✘                 | ✔                |                  |
| pyspark.sql.context                                | ✘                 | ✔                |                  |
| pyspark.sql.conf                                   | ✔                 | ✘                |                  |


## Disclaimer

Apache Spark, Spark, Apache, and the Spark logo are <a href="https://www.apache.org/foundation/marks/">trademarks</a> of
  <a href="http://www.apache.org">The Apache Software Foundation</a>. This project is not owned, endorsed, or sponsored by The Apache Software Foundation.
