Some articles I liked and what I took away from them (which I'll admit is not always the thesis of the article).

# General Development

## [Dan Luu on culture](https://danluu.com/culture/)
- Your personal limits are defined by the culture you're surrounded by, for better or for worse.
- Debugging habits are formed by who you learned to debug from, not so much your personal interest in diagnosing problems vs. fixing them fast.
- Onboarding matters way more than a highly technical screening process. (Subtext: hire the person you want, not the skills.)
- To that point, I won't copy-paste it, but Dan's appendix on how every hire impacts culture is perfect and really reflects my experience. I really feel each new person's immediate positive or negative impact on a team's attitude and temperature.

## [XY Problem](https://xyproblem.info/)
- Always present your question (Y) plus the pressures that brought you to that specific question (X). Too many times, Y didn't really follow from X and that critical info helps people with more context save you from yourself.

## [Law of Demeter](https://www2.ccs.neu.edu/research/demeter/demeter-method/LawOfDemeter/general-formulation.html)
- Good guideline for maintaining low coupling between components. Generally: methods should keep an interface specific to their needs and not pull in entire objects that they then have to deconstruct. They "ask" for what they need via their interface and callers give them the pieces that are required.

# Ruby/Rails

## [Thoughtbot's timezones post](https://thoughtbot.com/blog/its-about-time-zones)
- Leave things as UTC for as long as possible, preferably until they need to be presented to the user.
- Boy, timezones are hard.
- Thanks, Adam!


