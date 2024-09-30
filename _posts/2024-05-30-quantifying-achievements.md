---
layout: post
title: "How to add numbers to your resume"
---

# How to add numbers to your resume
## A Software Developer's guide to quantifying your impact

One of the most common pieces of feedback I got on my resume while I was student was to add numbers to help quantify the achievements on my resume but I had no idea how to do so.
Some people have told me with straight face that you can estimate, guess, or make up these number but this never really sit right by me.
After working as a developer for two years, I've learned few ways to do so that I'd love to share!

As a software developer there are broadly two types of impact you can focus on: software quality or performance and business metrics.

### Software Metrics

Two key ways to gather these software metrics are observability tools and benchmarks.

Usually when I think of quantifiable software achievements, I think of things like speeding up the response time of an endpoint or reducing the number errors within the system (similar to the [RED metrics](https://grafana.com/blog/2018/08/02/the-red-method-how-to-instrument-your-services/) for system observability).

If you increased that number of requests your web server can handle per second that's great!
But try to find or track some metrics that will help you prove this.

If you're working for a company, hopefully they have observability infrastructures already but if they don't or you're just working on a personal project you can look into some popular libraries for generating metrics including [OpenTelemetry](https://opentelemetry.io/), [StatsD](https://github.com/statsd/statsd) and [Prometheus](https://prometheus.io/docs/concepts/metric_types/).
These are often used in conjunction with tools such as [Datadog](https://www.datadoghq.com/) or [Grafana](https://grafana.com/) to visualize and alert on these metrics.

The observability methodology is great if your software is being deployed and used by an already large user base but sometimes your don't have enough users to get a reliable read.

A great alternative can be well designed benchmarks. Most languages have packages that allow you to run benchmarks on different implementations of code. This way if you improve the performance of a function for example, you can provide a real, tested number on exactly how much you improved it by.

### Business Metrics

If you're writing a resume, you're likely looking to get a job in an organization that cares more about profit and costs over things like time complexity of your function.
As such, we must enter the world of business metrics.

Suppose you added a new feature to the product your worked on. Congratulations! To capture the impact of this accomplishment you should ask yourself questions such as

- how many people use this feature?
- what does this feature enable users to do?
- how does this affect user acquisition, profit, or expenses?

Some of these can be tracked quite easily by running a few SQL queries but other times it's difficult to identify the more downstream impact. Here I recommend using the underrated skill of just talking to people. Product managers, engineering managers, business analysts and data scientists will be some of best resources.


Before starting a project, these key stakeholders have likely already scoped out the quantifiable business impact or perhaps will be the ones creating reports to summarize the findings or results from the project. 
This means they don't need to any extra work, they just need to share their findings with you.
These key people can help you identify the higher level business impact of your project, feature, or bug fix which you can then steal and put in your brag doc or resume!

---

I hope that these tips help! Let me know if you'd be interested in a tutorial of setting up some observability tools for your project!
