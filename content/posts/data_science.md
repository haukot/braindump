+++
title = "Data Science"
author = ["Jethro Kuan"]
lastmod = 2020-07-17T00:55:23+08:00
draft = false
+++

## Twitter Data Science Event {#twitter-data-science-event}

### Maya Hari, Twitter Managing Director APAC {#maya-hari-twitter-managing-director-apac}

> World's largest collection of human thought

Indonesia's flood relief effort empowered by geolocated tweets.

Half of the world's millennials will be in Asia by 2020. Asia is a
great canvas for solving and innovating on problems, making Asia an
engine for growth for Twitter.

Transliteration and languages are the next frontier of opportunity.

### Miguel Rios, Data Science lead at Twitter {#miguel-rios-data-science-lead-at-twitter}

[Twitter #interactive visualizations](https://interactive.twitter.com/)
[The Data Science Venn Diagram — Drew Conway](http://drewconway.com/zia/2013/3/26/the-data-science-venn-diagram)

{{< figure src="/ox-hugo/Data_Science_VD_2018-12-06_19-05-38.png" >}}

<!--list-separator-->

- Data Science Organization in Twitter

  1.  Foundational Data Science work
  2.  Growth Team
  3.  Habits Team
  4.  Health/Metrics Team

<!--list-separator-->

- Product Data Science Lifecycle

  Opportunity Sizing -> Testable Hypotheses -> Experiment & Design ->
  Instrumentation & Metrics -> Experiment Review -> Post-release
  Check-ins

  - Experiment review includes analyzing user behaviour, to come up with
    new ideas

### Diana Macias, Client Engineering Manager {#diana-macias-client-engineering-manager}

<!--list-separator-->

- 140 character limit story

  - 2016: Timing wasn't right for going beyond 140
  - Email sent by a Japanese engineer (Iku) previously iOS engineer,
    now on machine learning team:
    - From personal research project, Japanese characters need 140 characters, but English users need
      280-300 characters
    - Japanese can contain about 1.9x more information than English in a
      character, visualized by separating tweets by language
    - Japanese plain tweet length averages around 14 characters
    - Tweet lengths fit a log-normal distribution: extending the
      log-normal distribution for english, 280 characters is the number found.
  - The 280 character project was born, customizing character limit
    based on the keyboard.
  - 9% of tweets hit the 140 limit, 1% of the tweets hit the 280 limit
  - Post analysis of 280 project:
    - Less abbreviations
    - More kind words like "please", "thank you"
    - Same tweet length

### Angad Singh, Data Science Team Lead, Twitter SG {#angad-singh-data-science-team-lead-twitter-sg}

<!--list-separator-->

- Twitter SG Data Science Team

  - small team of 5 data scientists
  - focused on user behaviour and international growth
  - experimentation on Android/iOS/Web

<!--list-separator-->

- 3Vs of data at Twitter

  - **Velocity**: Rate at which data is created
    - Hundreds of millions of Tweets are sent per day. TPS record:
      one-second peak of 143,199 Tweets per second
    - Order of 100B interaction events per day
  - **Volume**: 100s of petabytes of data
  - **Variety**: Tweets, Users, LIkes, Retweets and many more

  Production Systems

  - Batch (Hadoop, HDFS, MapReduce)
  - Real-time (Eventbus, Kafka Streams)

  Analytics Tools

  - Batch: Scalding, Spark
  - Real-time: Heron
  - Lambda (Batch + Real-time): Summingbird, TSAR
  - Interactive: Presto, Vertica, R

  Analytics Front-ends

<!--list-separator-->

- Hadoop

  - Some of the largest Hadoop clusters in the world: > 10k nodes
  - Store 100s of peabytes of data
  - More than 100k daily jobs
  - [twitter/ambrose](https://github.com/twitter/ambrose) for visualizing Hadoop jobs

<!--list-separator-->

- Core Data Libraries

  - [twitter/scalding](https://github.com/twitter/scalding): DSL on top of Cascading (Java library for MapReduce)
  - [twitter/summingbird](https://github.com/twitter/summingbird): Lambda architecture: real-time and batch

<!--list-separator-->

- Interactive SQL

  - Interactive means that results of a query are available from the
    range of seconds to couple of minutes
  - SQL still lingua franca of ad-hoc data analysis:
    - Presto
    - HP Vertica
    - Google BigQuery

<!--list-separator-->

- Data Visualization:

  - Apache Zepplin
  - Tableu

<!--list-separator-->

- Data Insights

  - Analytics - Basic Counting
  - A/B Testing
  - Data Science - Exploratory Analysis
  - Data Science - Machine Learning

<!--list-separator-->

- Basic Counting

  - Daily/Monthly Acitve Users
  - Number of Tweets

<!--list-separator-->

- Data Science - Custom Analytics

  - Cause of spikes and dips in main metrics

<!--list-separator-->

- Machine Learning

  - Recommendations
    - Users: Who to follow
    - Tweets: Algorithmic timeline
  - [Cortex](https://cortex.twitter.com/en.html), DL based on Torch framework (now Tensorflow)
    - Identify NSFW images
    - Recognize what is happening in live feeds

<!--list-separator-->

- Ideal Talent Stack

  - Systems (Hadoop, Distributed Systems)
  - Programming (Scala, Scalding, SQL)
  - Math (Statistics, Linear Algebra)
