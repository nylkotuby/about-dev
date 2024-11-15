# Observability

You can't know if something works or not if you can't observe it. Just as bad, if your system is insufficiently observable and monitored, your customers are doing your monitoring for you - and that has a high cost and long tail.

I'm not necessarily using industry terms in this brain dump, just how I personally classify things after doing a good bit of observability work as an infra and backend engineer. If you know of better industry terms for these concepts, I'd love to hear them.

## Noisy alerts are worse than no alerts at all

If you have lots and lots of alerts that are meaningless - outdated, unspecific, trip too early, or are otherwise largely or completely ignored by engineers - these are worse than having no alerts at all. They drown out any important alerts that you might still have around and quickly lead to alert fatigue and burnout.

When a team is experiencing alert fatigue, I genuinely think it's better to mute (or even better, delete) any alert that you cannot 100% justify/explain/understand than to keep it around "just in case". If it's monitoring something important, you _will_ create the alert again.

A bad alert makes a difficult-to-measure but nonetheless real impact on your team's ability to assess risk and the health of your system, the cost of which far outweighs any perceived value.

## Engineering metrics

"Engineering metrics" are how I refer to measurements made on resources or flows that are scoped to the interest of the engineering team only. They probably don't correlate to a specific feature, product goal, or marketing funnel - they're generally more scoped to pieces of infrastructure, points of data ingress/egress, or particular applications (or groups of applications). This level of technical granularity isn't of general interest to folks outside of engineering, but having good metrics for these systems gives us the "why" and "how" for product performance & problems.

Some people prefer to lead with business metrics, but in my opinion, monitoring business metrics without having a solid foundation for the systems that underly them is a losing game. If I get a page that says "Payment system isn't working" without knowing if the frontend is being served, the database is down, or our payments partner is unreachable, I have to:
    1. know personally that all of those things are part of our payments flow (not every engineer can have full knowledge of every system)
    2. validate all of those things on my own before I can start fixing the problem

On the other side of things, if I get a page saying "Database is down", I may not know all the specific things in our app that the database powers, but I can make a pretty good guess that it's affecting a few things, and I know exactly where to start my diagnosis.

### Critical engineering metrics

Is this queue full?
Is this app down?
Is this connection down?
Am I timing out?

### Non-critical engineering metrics (or performance metrics)

Is this job retrying often?
Is this traffic volume too high?

Allows for tuning things to be faster, cheaper (scaling), more responsive

## On-call

## Business metrics


