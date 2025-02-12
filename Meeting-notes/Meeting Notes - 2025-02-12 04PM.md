## Attendees
Rene
## Agenda
### 1. Updates
- Rene put some work in on the PR we were working on today for [WB-17781](https://app.clickup.com/t/86dvx7qwe)
### 2. Discussion Points
- Talked about some funky Go string casting rules
- Discussed final changes to [WB-17781](https://app.clickup.com/t/86dvx7qwe), is ready now
- Went over next work for me, [WB-17906](https://app.clickup.com/t/8593290/WB-17906)
## Action Items
- Begin work on [WB-17906](https://app.clickup.com/t/8593290/WB-17906)
## Key Notes
- Make sure to use `fmt.Sprint()` for string conversions, `string()` casting gives unintended consequences
- Make sure to make a new branch to work on 17906!