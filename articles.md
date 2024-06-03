Some articles I liked and what I took away from them.

Also some articles I find myself repeatedly looking up to share w/others because they describe common principles I follow or use. (Usually impressed upon me by the great dev team at Upserve.)

# General Development

## [x](https://danluu.com/culture/) Dan Luu on culture
- Your personal limits are defined by the culture you're surrounded by, for better or for worse.
- Debugging habits are formed by who you learned to debug from, not so much your personal interest in diagnosing problems vs. fixing them fast.
- Onboarding matters way more than a highly technical screening process. (Subtext: hire the person you want, not the skills.)
- To that point, I won't copy-paste it, but Dan's appendix on how every hire impacts culture is perfect and really reflects my experience. I really feel each new person's immediate positive or negative impact on a team's attitude and temperature.

## [x](https://xyproblem.info/) XY Problem
- Always present your question (Y) plus the pressures that brought you to that specific question (X). Too many times, Y didn't really follow from X and that critical info helps people with more context save you from yourself.

## [x](https://www2.ccs.neu.edu/research/demeter/demeter-method/LawOfDemeter/general-formulation.html) Law of Demeter
- Good guideline for maintaining low coupling between components. Generally: methods should keep an interface specific to their needs and not pull in entire objects that they then have to deconstruct. They "ask" for what they need via their interface and callers give them the pieces that are required.

# Ruby/Rails

## [x](https://thoughtbot.com/blog/its-about-time-zones) Thoughtbot's timezones post
- Leave things as UTC for as long as possible, preferably until they need to be presented to the user.
- Boy, timezones are hard.
- Thanks, Adam!


