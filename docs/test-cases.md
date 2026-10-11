# Home Credit LAP Voice Agent — Test Cases

## Objective

Validate the voice agent's conversation flow, preliminary eligibility rules, exception handling, and call termination behavior using fictional test data.

## Test Results

| ID | Test Scenario | Expected Behavior | Result |
|---|---|---|---|
| TC-01 | All seven eligibility checks pass | Agent explains preliminary qualification and senior-expert follow-up | Passed |
| TC-02 | Agricultural property | Agent disqualifies the application and ends the call | Passed |
| TC-03 | Requested amount exceeds ₹75 lakh; customer accepts the limit | Agent updates the requested amount to ₹75 lakh and continues | Passed |
| TC-04 | Requested amount exceeds ₹75 lakh; customer declines | Agent explains the limit and ends the call | Passed |
| TC-05 | Original property documents unavailable | Agent disqualifies the application and ends the call | Passed |
| TC-06 | Customer receives income in cash | Agent disqualifies the application and ends the call | Passed |
| TC-07 | Requested tenure is below 3 years | Agent disqualifies the application and ends the call | Passed |
| TC-08 | Requested tenure is 15 years | Agent accepts the tenure and continues qualification | Passed |
| TC-09 | Customer wants an existing loan transferred or wants to reduce EMI | Agent routes the request to a specialist and ends the current call | Passed |
| TC-10 | Customer is busy and requests a callback | Agent acknowledges the preferred time and ends the current call | Passed |
| TC-11 | Mock identity verification fails | Agent does not disclose the offer and ends the call | Passed |
| TC-12 | Customer provides eligibility answers out of order | Agent remembers valid answers and asks only for missing information | Passed |
| TC-13 | Customer has joint property ownership | Agent accepts joint ownership and continues qualification | Tested; verify full completion |

## Test Notes

- Tests use fictional customer information and mock verification data.
- Preliminary qualification is not final loan approval.
- The agent must not invent interest rates or property-value thresholds.
- Callback preferences must not be described as confirmed appointments unless a scheduling system confirms them.
- Test outcomes should be supported by the corresponding Retell call transcript or recording.

## Evidence

Retell AI call transcripts and recordings were collected for testing. Add individual call IDs or evidence links here only when they have been verified and are safe to share.

## Limitations

This project demonstrates a preliminary qualification conversation. It does not independently verify real customer identity, approve loans, calculate an official interest rate, or guarantee that a callback has been scheduled.
