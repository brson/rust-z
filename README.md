# Battleplan Rust

A *prototype* tool for organizing the activity of The Rust Project.

Rust is a huge effort. There's a lot going on. But it's difficult for
the casual observer - or even those deeply involved - to grasp the big
picture of where Rust is going, and how it will get there. This tool
is an attempt to improve the situation by collectiing key information
already produced by Rust's development process, and presenting it in
an easily-digestable format.

## Goals

- Give users and contributors a picture of what's happening in Rust
  and where it's going.
- Illuminate current project initiatives and the RFC feature pipeline.
- Inspire users and contributors with a common vision for the future.
- Progressive detail - on first glance one should sense the scope
  of the project, and the key deliverables for the coming releases
  across all corners of the project. Drilling down, both users
  and contributors should be able to discover detailed information
  about the state of the project's goals.
- Link all relevant issues, RFCs, pull reuests, etc. associated with
  any particular feature or initiative.
- Provide entry points for contributors.
- Foreshadow future initiatives and features.
- Demonstrate progress towards the project's goals.
- Visualize the finished and unfinished sub-tasks for any particular
  initiative.
- Show what's in the next release.
- Living updates - everybody can help maintain it.

## How?

Fundamentally, this tool helps organize the *tracking issues* already
produced by the Rust development process. Tracking issues of strategic
importance are registered with the tool as *goals*, and they are
stated as concrete, limited deliverables. The tool automatically
derives important data about the progress of each goal and
presents it to the user in a way that is easier to understand than
attempting to discover the same information through the usual GitHub,
etc. UI.

There are three major components to this:

- A data schema defined by yaml files in `_data`, curated by a human,
  and in `_data/gen`, generated by machine.
- A static webapp that presents that data.
- A Rust application that keeps the data up to date by scraping
  sources, and guiding the user to improve the data set.

It is intended that the manual curation is kept to a minimum, but
achieving that will be an ongoing matter of discovery, tool
improvement, and process improvement.

## Process implications

The quality of information we can present is only as good as the
quality of data generated by the Rust development process. In some
places - most notably RFC-driven features - that data is quite
complete already; in others we'll need to improve. But hopefully
making the changes necessary is mostly a matter of being more
consistent in our process, and the tool can be designed to help
discover places where the data is poor.

From what I've seen so far I think these are the places we need
to improve in order to make the right data available:



