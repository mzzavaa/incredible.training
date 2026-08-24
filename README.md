# incredible.training : Commercial Learning & Enablement Business

**Domain:** incredible.training
**Role:** Commerce : Courses, workshops, and cohort programmes sold as products
**Priority:** Phase 1
**Strategy doc:** internal, not linked from here

## Purpose
The learning business of the Incredible group. Sells named courses with published prices,
published dates, and stated outcomes, to two distinct buyers: L&D leads and engineering
managers buying enablement for a team, and individual engineers buying a seat. Where
consulting delivers a system, training leaves behind people who can build and run one.

This domain owns the catalogue, the curriculum, the trainers, the credentials, the calendar,
and the checkout. It is the second commercial destination in the portfolio after
incredible-consulting.com, and the only one that sells a productised, repeatable unit.

## Key Features / Sections
- Course catalogue with a dedicated page per course, including level, prerequisites, and price
- Four delivery formats: half day, multi day intensive, cohort programme, self paced
- Role-based learning paths with prerequisite sequencing and stated total cost
- Corporate and in-house training: private courses, enablement programmes, skills assessment
- Split buying journeys for teams and for individuals, priced and explained separately
- Trainer roster, qualification standard, and named-trainer guarantee for private bookings
- Certification and credentials with published assessment criteria and public verification
- Schedule with confirmed dates, seat counts, waitlists, and a request-a-date route
- Published pricing, including the break-even between private delivery and open seats
- Procurement, invoicing, and third-party funding routes
- FAQ split by buyer type, and a booking hub that routes by intent

## Monetization
Direct. Three revenue lines: individual course fees and cohort seats, private in-house
course delivery charged on a day rate, and corporate enablement contracts charged as a fixed
programme fee with milestone invoicing. Secondary lines: self paced team licences, skills
assessments (credited against a programme), and reassessment fees.

## Content map

```
content/
  _index.md                                Homepage
  courses/
    _index.md                              Course catalogue
    ai-agents-in-production.md             AGT-300, advanced, 3 days
    genai-foundations-for-engineers.md     GEN-100, foundation, 2 days
    rag-and-knowledge-systems.md           RAG-200, intermediate, 2 days
    cloud-foundations-on-aws.md            CLD-100, foundation, 3 days
    ai-governance-and-the-eu-ai-act.md     GOV-200, intermediate, 1 day
    ai-for-managers.md                     MGT-100, foundation, half day
  formats/
    _index.md                              Format comparison and trade-offs
    half-day.md                            Alignment and decision support
    multi-day-intensive.md                 The default technical format
    cohort-programme.md                    Six to eight weeks, part time, capstone
    self-paced.md                          Recorded modules and labs
  learning-paths/
    _index.md                              Role-based routes through the catalogue
    ai-engineer.md                         GEN-100 to RAG-200 to AGT-300
    cloud-platform.md                      Platform and infrastructure route
    technical-leadership.md                Manager and decision-maker route
    curriculum-and-levels.md               Instructional design, levels, review cadence
  for-teams/
    _index.md                              The corporate buying page
    in-house-training.md                   Private delivery of catalogue courses
    enablement-programmes.md               Multi-course programmes with measurement
    skills-assessment.md                   Diagnostic that precedes a programme
    procurement-and-invoicing.md           Entity details, terms, documents
  for-individuals/
    _index.md                              The self-funded buying page
    seats-and-enrolment.md                 Booking mechanics and joining pack
    scholarships-and-community-rates.md    Reduced and free seats
    learner-support.md                     Office hours, alumni access, escalation
  trainers/
    _index.md                              Roster and the trainer standard
    linda-mohamed.md                       Lead trainer and curriculum owner
    associate-trainers.md                  Vetting, scaling, substitution policy
    become-a-trainer.md                    Associate roster recruitment
  certification/
    _index.md                              What the credentials mean
    credential-catalogue.md                Every credential and its evidence
    assessment-and-exams.md                Assessment design and marking criteria
    verify-a-credential.md                 Employer verification lookup
  schedule/
    _index.md                              Calendar and list of open dates
    upcoming-dates.md                      Full six month listing and run thresholds
    request-a-date.md                      Demand capture for unlisted dates
  pricing/
    _index.md                              Published price overview
    individual-seats.md                    Per-seat and per-cohort prices
    team-and-corporate.md                  Private, programme, and seat block pricing
    funding-and-subsidies.md               Austrian, EU, and vendor funding routes
  book/
    _index.md                              Booking hub, routed by intent
    enrol-in-a-course.md                   Individual checkout flow
    request-a-team-quote.md                Corporate quote capture
  faq/
    _index.md                              Questions grouped by who is asking
    courses-and-curriculum.md              Content, prerequisites, tooling, currency
    booking-and-cancellation.md            Payment, transfers, refunds, no-shows

data/
  courses.yaml                             Course registry driving catalogue and pricing
  schedule.yaml                            Scheduled runs, seats, and status
  trainers.yaml                            Trainer roster and named-trainer assignment
  credentials.yaml                         Credential registry and badge metadata
```

## Relationship to other Incredible domains

| Domain | Relationship |
| --- | --- |
| incredible-company.com | Group parent. Carries the legal entity, trust centre, and press assets that procurement asks for. This site links to the trust centre rather than restating security and data protection. |
| incredible-consulting.com | The canonical consulting domain and the closest commercial neighbour. The boundary is stated on the homepage and repeated on course pages: buy training when you want capable people, buy consulting when you want a delivered system. Course pages link out to the matching service; consulting engagements link back for team enablement. |
| incredible-consulting.org | Open methodology and public-good arm. Source of the published frameworks and governance templates the curriculum draws on. /learning-paths/curriculum-and-levels/ credits it instead of republishing the material. |
| incredibleconsulting.org | Typo-catch and defensive domain. No relationship beyond the portfolio record; nothing here links to it. |
| incredible.builders | Practitioner and open source community. Where most associate trainers are recruited and where alumni continue after a course. Owns the repositories and contribution guides, so this site links rather than hosts them. |
| incredible.community | People, events, and membership. Owns the meetup calendar and member directory. Community members get a reduced seat rate; the events calendar there and the course schedule here stay separate. |
| lindamohamed.work | Founder's personal portfolio. /trainers/linda-mohamed/ summarises the practitioner record and links out for the full speaking and consulting history. |
| ai-workshops.online | Existing sibling property carrying the Three Workshop Method as a consulting-led discovery format. Distinct from this catalogue: that is a delivery engagement shape, this is a productised curriculum. Kept separate to avoid two prices for one thing. |

**Rule of thumb.** This domain sells learning. If the visitor wants someone else to build the
system, it belongs to incredible-consulting.com. If they want the open framework for free, it
belongs to incredible-consulting.org. If they want people to hang around with, that is
incredible.builders and incredible.community. Everything here has a price, a date, and a
named trainer.

## Local development

```
make dev      # hugo server on the first free port from 1313
make build    # hugo --gc --minify
make clean    # remove public, resources/_gen, .hugo_build.lock
```

Theming is a later pass. `layouts/` and `static/` are intentionally empty.

## House style

No em-dashes, no emojis, anywhere in this repository. Voice is direct, concrete, and
practitioner-level. Prices, durations, and prerequisites are stated rather than hidden behind
a contact form. Brand palette for the theming pass: green #3D8F37 · dark #0a1a08 · white #fff
· background #f8f9f6. Font: Inter.
