# AgentCollect

## Frame
Debtor pages - relucant users, hestitation
Client dashboard - Users who uses platform daily

## Assumptions

- Recording sample - 80% or more
- Rage click / dead click / console error logging
- No A/B testing
Goal: Detector which scales without increasing headcount
- Input mask is on

## Sources / GT

- Model path / Happy flow (same device, same OS, same page, same entry point)
    - 100 users out of which 3 are deviating
- recurrance (many points == signal)
- Outcome correlation - intent scoring

Note: We need multiple or atleast 2 signals supporting to move forward.

- Dead clicks - No DOM, No network response
    - We check logs at same time
- abondon-after-interaction - pair this with intent score
- Console error at same time of rage clicks or no network/ no dom change at time of multiple clicks
- Loop - same pages

Score = signal x recurrance x outcome

## Privacy

- Unmasked data is not desired
- Element role, signal type, timestamps - abstract data with no personal information