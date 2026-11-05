# GSU Interdisciplinary Studies

Scenario-based assessments (SBAs) for an interdisciplinary studies course
developed at Georgia State University. Students investigate a social problem
through multiple disciplinary lenses, working through research studies,
focus group transcripts, and comparison activities presented as interactive
SMS-style conversations with a simulated team.

## Content

The repository holds two SBAs:

- **Homelessness SBA** (`homelessness/`), the one deployed. The student
  interns at Comm360, a local nonprofit, and with fellow interns investigates
  the causes of homelessness. It has three parts; Part 1 (`part1/`) is here
  now, and Parts 2 and 3 will be added as `part2/` and `part3/`. Files shared
  by all parts (the manifest, the course `hs_course.olx`, and the consent
  gate) sit at the top of `homelessness/`.
- **High-school-dropout SBA** (`high-school-dropout/`), the earlier SBA:
  three parts analyzing the high school dropout crisis. It is kept in the
  repository but not currently deployed. All three parts are in its course
  (`interdisciplinary_course.olx`); Parts 2 and 3 carry `when="false"`, which
  keeps them out of the navigation.

Each part combines a ChatPEG dialogue, an activities file, and supporting
readings (under its `readings/` folder).

The readings are short course summaries of published research. Each one names
the original, so you can read the whole thing. Focus-group transcripts and
similar scenario materials are different: they were written for the scenario,
and the people and numbers in them are made up.

To hide a part until it is released, give its `<Use>` in the course
`when="false"`; to release it, delete the `when="false"` and redeploy the
content.

## Research study

Each SBA's route `/` (its `manifest.yaml`) lands on a research-study gate
(`homelessness/hs_study.olx`; `high-school-dropout/interdisciplinary_study.olx`),
which shows the informed-consent form first (`consent.olx`). Either answer,
accepting or declining, leads into the course; the activities and credit are
the same. Students can change their answer at any time from **Study Consent
Form** at the bottom of the course navigation. For a deployment outside the
study, point `/` at the course (`homelessness/hs_course`) instead.

---

The author catalog reads this README for the repository description (git
conventions first; `lo.yaml` covers only beyond-git fields like discipline).
Licensing and attribution live in `LICENSE.TXT`, `NOTICE.TXT`, and
`CONTRIBUTORS.TXT`.
