---
layout: post
title: "How to add numbers to your resume"
---

# How to add numbers to your resume
## A Software Developer's guide to quantifying your impact

One of the most common pieces of feedback I got on my resume while I was a student was to add numbers to help quantify the achievements but I had no idea how to do so.
Some people have told me with a straight face that you can estimate, guess, or make up these numbers but this never really sat right by me.

After working as a developer for two years, I've learned a few ways to quantify my achievements that I'd love to share!

Two types of quantifiable metrics you can broadly focus on are software quality or performance and business metrics.

### Software Metrics

Two key ways to gather software metrics are observability tools and benchmarks.

Usually, when I think of quantifiable software achievements, I think of things like speeding up the response time of an endpoint or reducing the number of errors within the system (similar to the [RED metrics](https://grafana.com/blog/2018/08/02/the-red-method-how-to-instrument-your-services/) for system observability).

If you increased the number of requests your web server can handle per second that's great!
But try to find or track some metrics that will help you prove this.

If you're working for a company, hopefully, they have observability infrastructure already but if they don't or you're just working on a personal project you can look into some popular libraries for generating metrics including [OpenTelemetry](https://opentelemetry.io/), [StatsD](https://github.com/statsd/statsd) and [Prometheus](https://prometheus.io/docs/concepts/metric_types/).
These are often used in conjunction with tools such as [Datadog](https://www.datadoghq.com/) or [Grafana](https://grafana.com/) to visualize and alert on these metrics.

The observability methodology is great if your software is being deployed and used by an already large user base but sometimes you don't have enough users to get a reliable read.

A great alternative can be well-designed, statistically significant benchmarks. Most languages have packages that allow you to run benchmarks on different implementations of code. This way if you improve the performance of a function, you can provide a real, reasonable number to back up your claims. Some such libraries are [benchmark-ips](https://github.com/evanphx/benchmark-ips) for Ruby, Python's [timeit](https://docs.python.org/3/library/timeit.html) module, or [criterion.rs](https://github.com/bheisler/criterion.rs) for Rust.

### Business Metrics

If you're writing a resume, you're likely looking to get a job in an organization that cares more about profit and costs over things like the time complexity of your function.
As such, we must enter the world of business metrics.

Suppose you added a new feature to the product you worked on—congratulations! To capture the impact of this accomplishment you should ask yourself questions such as, but not limited to

- How many people use this feature?
- What does this feature enable users to do?
- How does this affect user acquisition, profit, or expenses?

Some of these can be tracked quite easily by running a few SQL queries but other times it's difficult to identify the more downstream impact. Here I recommend using the underrated skill of just talking to people. Product managers, engineering managers, business analysts and data scientists will be some of your best resources.


Before starting a project, these key stakeholders have likely already scoped out the quantifiable business impact or perhaps will be the ones creating reports to summarize the findings or results from the project. 
This means they don't need to do any extra work, they just need to share their findings with you.

It's important to have an understanding of which metrics your company cares about at the moment. Common ones are gross profit (GP), daily active users (DAU), and monthly recurring revenue (MRR) but there are many more!

One challenge you might face is that changes in these metrics can sometimes be attributed to multiple factors, making it hard to isolate the impact of your specific feature. 
In such cases, running an A/B experiment can be a powerful way to measure the effect of your feature alone.
Collaborating with data scientists or analysts and getting buy-in from your manager can help you set up an experiment that clearly ties the results to your work.

These key people can help you identify the higher-level business impact of your project, feature, or bug fix which you can then steal and put in your [brag doc](https://jvns.ca/blog/brag-documents/) or resume!

---

I hope that these tips help! 
Being relatively new to the industry, I'm sure there are methods and metrics that I've missed. Please [leave a comment on HN](https://news.ycombinator.com/item?id=41848978) and let me know what those things are!
