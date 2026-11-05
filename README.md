# GSU Interdisciplinary Studies

A scenario-based interdisciplinary studies course developed at Georgia State
University. Students analyze the high school dropout crisis through multiple
disciplinary lenses — education, sociology, economics, public health — using
research studies, focus group transcripts, and concept-mapping activities
presented as interactive SMS-style conversations.

## Content

The course is a three-part scenario-based learning activity (SBLA):

1. **Part 1** — orientation to the dropout problem and initial research review
2. **Part 2** — concept mapping with Mermaid diagrams and deeper analysis
3. **Part 3** — synthesis and interdisciplinary integration

Each part combines a ChatPEG dialogue, an activities file, and supporting
readings under `high-school-dropout/readings/`.

The readings are short course summaries of published research. Each one names
the original and links to it, so you can read the whole thing. The focus-group
transcript and the policy brief are different: they were written for the
scenario, and the people and numbers in them are made up.

All three parts are in the course (`interdisciplinary_course.olx`), but Parts
2 and 3 are present and hidden until released: each carries `when="false"`,
which keeps it out of the navigation. To release a part, delete its
`when="false"` and redeploy the content.

## Research study

The deployment's route `/` (`high-school-dropout/manifest.yaml`) lands on the
research-study gate (`interdisciplinary_study.olx`), which shows the
informed-consent form first (`consent.olx`). Either answer, accepting or
declining, leads into the course; the activities and credit are the same.
Students can change their answer at any time from **Study Consent Form** at
the bottom of the course navigation. For a deployment outside the study,
point `/` at `interdisciplinary_course` instead.

---

The author catalog reads this README for the repository description (git
conventions first; `lo.yaml` covers only beyond-git fields like discipline).
Licensing and attribution live in `LICENSE.TXT`, `NOTICE.TXT`, and
`CONTRIBUTORS.TXT`. The courseware itself is under `high-school-dropout/`
(not currently deployed).
