# Progress

## Projects

| # | Days | Project | Roles | Status | Live | Repo |
|---|---|---|---|---|---|---|
| 1 | 1–2 | FlowPlan: project scheduler with critical path | Dev · PM | ✅ Done (v1.1) | [flow-plan-five.vercel.app](https://flow-plan-five.vercel.app/) | [FlowPlan](https://github.com/ahmed-malikk/FlowPlan) |
| 2 | 3–5 | QueueCare: clinic queue & appointments | Dev · BA · PM | ✅ v1.0 released (gist check and pilot open) | [queuecare-zeta.vercel.app](https://queuecare-zeta.vercel.app) | [QueueCare](https://github.com/ahmed-malikk/QueueCare) |
| 3 | 6–7 | Local Business BA Case Study | BA | Not started | – | – |
| 4 | 8–10 | CommitteeKeeper: savings committee tracker | Dev · BA · PM | Not started | – | – |
| 5 | 11–12 | PulseMetrics: product analytics | Dev · PM | Not started | – | – |
| 6 | 13 | Product Teardown + Roadmap | PM | Not started | – | – |
| 7 | 15–17 | LudoLive: online multiplayer Ludo | Dev | Not started | – | – |
| 8 | 18–19 | RouteRider: delivery route planner | Dev · BA | Not started | – | – |
| 9 | 20 | HireTrack: job tracker + skill-gap analyzer | Dev · PM | Not started | – | – |
| 10 | 21 | Portfolio Site + Program Report | PM | Not started | – | – |

## Log

- **2026-10-07 · FlowPlan v1.0 shipped.** Live on Vercel; [release notes](https://github.com/ahmed-malikk/FlowPlan/releases/tag/v1.0). 44/44 unit tests, 42/42 system tests (Edge, Chrome, 375 px phone) on the local build and the live site. Testing found and fixed 2 phone layout bugs. 13 issues, 12 closed. **Still open:** gist check, usability test with 3 people, my own 3-week plan in FlowPlan ([#10](https://github.com/ahmed-malikk/FlowPlan/issues/10)). **Next:** QueueCare.
- **2026-10-07 · FlowPlan v1.1.** Added mark-as-done and task notes; long dependency lists now scroll (#14–#16). 51/51 unit and 51/51 system tests, locally and on the live site. Loaded my one-person sprint plan (21 days, every project critical) for issue #10.
- **2026-10-07 · FlowPlan done for the 3-week plan.** All 16 issues closed. Real use: my own sprint planned in FlowPlan finishes on day 21 with all 11 items critical (12 days on dependencies alone; the gap is me being one person). Still open, not blocking: usability test with 3 people, print layout polish, a GitHub Project board. **Next:** gist check, then QueueCare.
- **2026-10-07 · FlowPlan gist check done.** Walkthrough of `scheduler.ts` explained back (6.5/10), then the 3 checkpoint questions: critical path and why a PM cares (6/10), loop detection (7.5/10), slack and delays (9/10). To improve: slack is an output, tasks are nodes and dependencies are edges, critical tasks are the ones to protect. Practise the answers out loud once more without notes.
- **2026-10-07 · FlowPlan lessons learned written:** [docs/lessons/flowplan.md](docs/lessons/flowplan.md). Technologies, structure, testing, GitHub, deployment, teamwork, PM insights, and 6 changes for QueueCare.
- **2026-10-07 · QueueCare Day 0.** Repo created; plan in README; stakeholder interview guides written (receptionist, patients); labels ready. Next: interviews, BRD, PRD (Thu 8 Oct).
- **2026-10-07 · QueueCare interviews.** One receptionist and three patients in Lahore; [findings](https://github.com/ahmed-malikk/QueueCare/blob/main/docs/research/interview-findings.md). Not knowing how long the wait is hurts more than the wait itself (4 of 4). BRD (27 requirements) and PRD (9 stories) written the same day.
- **2026-10-09 · QueueCare v1.0 shipped (day 4 of a 3-day slot ending day 5).** Live at [queuecare-zeta.vercel.app](https://queuecare-zeta.vercel.app); [release notes](https://github.com/ahmed-malikk/QueueCare/releases/tag/v1.0). All six Must stories: staff roles, registration with QR tokens, priority queue with urgency changes, Call next with live updates, patient status page without an account, waiting-room display. 77/77 unit tests, 16/16 security checks, 23 system test cases on Edge, Chrome and a 375 px phone, passing locally and on the live site. Live updates 0.8–0.9 s (target 2 s); patient page 2.3 s on throttled mobile data (target 3 s). Seven defects found and fixed. Should stories (#10–#12) moved to the backlog. **Still open:** gist check, real-phone check, pilot at a clinic. Lessons: [docs/lessons/queuecare.md](docs/lessons/queuecare.md).
- **2026-10-09 · QueueCare gist check done.** The 3 checkpoint questions: why not just sort when someone joins (6/10: priorities change with time, so the order is recomputed on every load; missed the failure case and why it's cheap), stopping a low-urgency patient waiting forever (8/10: aging, +1 level per 30 min up to Urgent; add the arrival tie-break and the Emergency cap), what the receptionist changed (6/10: "how much longer?" → wait estimates; add stepping out → live status page, informal priority → written rules, the existing TV → waiting-room display). To improve: answer with point → example → why it matters.
