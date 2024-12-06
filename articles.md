I find myself frequently looking these articles up to share with others. They (or the principles they describe) have been very influential to me, so I like having them in one place to be able to easily reference. Also including some notes about what I liked or took away from the reading.

# General Development

## [x](https://xyproblem.info/) XY Problem
- Always present your question (Y) plus the pressures that brought you to that specific question (X). Too many times, Y didn't really follow from X and that critical info helps people with more context save you from yourself.

## [x](https://www2.ccs.neu.edu/research/demeter/demeter-method/LawOfDemeter/general-formulation.html) Law of Demeter
- Good guideline for maintaining low coupling between components. Generally: methods should keep an interface specific to their needs and not pull in entire objects that they then have to deconstruct. They "ask" for what they need via their interface and callers give them the pieces that are required.

## [x](https://conventionalcomments.org/) Convential Comments
- Framework for tagging comments for clarity. The quality of my PR review immediately increased when I started using these tags.
- I realized recently that stopping to think about what tag I want to use is half the battle. Why should the PR author have to decipher my intent for me?

# Ruby/Rails

## [x](https://thoughtbot.com/blog/its-about-time-zones) Thoughtbot's timezones post
- Leave things as UTC for as long as possible, preferably until they need to be presented to the user.
- Boy, timezones are hard.
- Thanks, Adam!


# Process & People

## [x](https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals) GitLab on "directly-responsible individuals"
- People who are doing the work and accountable for its completeness should be the ones who make the ultimate decisions for how the work is done.
- This does not absolve them of the hard work of consulting with and informing folks, but is just a framework for "tiebreaking" and breaking up logjams of endless discussion. I've been a part of so many teams that verbalized a wish to move faster, but focused deeply on consensus-building where it (in my opinion) wasn't called for.
- The article makes a great point about how having to explain yourself too much and too often can force people to operate in secret, which this framework of course also explicitly sets out to address.


## [x](https://danluu.com/culture/) Dan Luu on culture
- Your personal limits are defined by the culture you're surrounded by, for better or for worse.
- Debugging habits are formed by who you learned to debug from, not so much your personal interest in diagnosing problems vs. fixing them fast.
- Onboarding matters way more than a highly technical screening process. (Subtext: hire the person you want, not the skills.)
- To that point, I won't copy-paste it, but Dan's appendix on how every hire impacts culture is perfect and really reflects my experience. I really feel each new person's immediate positive or negative impact on a team's attitude and temperature.

