# Save a customer journey as a focus

- Read this reference only when creating or changing a shopper's area of focus.
- The customer supplies the goal; the examples illustrate possible briefs, not mandatory steps or recorded tests.

## Preserve the saved shopper

- `save_assignment` replaces the supplied focus list.
- Omit `focus` to preserve it, and use an empty list only when removing all focus is requested.
- Read the current list, retain existing items when adding one and preserve every unchanged shopper setting.
- If the focus field is unavailable, do not send a replacement list.
- The same item listed twice is kept once.

## Focus fields

Each focus item supports:

| Field | Meaning |
| --- | --- |
| `intent` | What to do, 12–600 characters |
| `startingUrl` | Optional full HTTP(S) start page supplied for the task |
| `successDescription` | Optional visible success, at most 300 characters |
| `when` | `one_time` for the next admitted check, or `going_forward` for future checks until removed |

## What saving a focus does

- A one-time item leaves the list once a check carrying it has been admitted, not when a successful result is published.
- Saving the focus starts no check.
- No tool runs one focus alone.
- A basic recheck uses the first saved non-retired shopper, which may be a different shopper; disclose that before requesting a check.

## Write the focus

- Use the user's wording and supported schema.
- If one-time versus ongoing would change their request and is unclear, ask that choice.
- Do not invent a private login, a business rule, a start URL or an unstated success condition.
- Use an explicit user goal or returned page evidence; clarify only a material ambiguity.

## Example briefs

- Adapt an example to the requested flow and visible success.
- Include a starting URL when the user supplies it or returned page evidence establishes the requested starting point; otherwise omit it.

| Customer task | Example intent | Example visible success |
| --- | --- | --- |
| Signup and first use | Create a test account, finish the setup questions and save the first project. | The project remains saved and its detail screen opens. |
| Consumer web application | Answer the setup questions and open the first personalized plan. | The plan shows the selected preferences and opens its next step. |
| Contact or demo form | Complete the contact form and check whether Continue opens its confirmation. | The confirmation is visible and required-field errors identify the relevant field. |
| Mobile checkout | On the recorded mobile view, choose an item and proceed from the cart to the shipping choices. | The cart retains the selected item and the shipping choices are usable. |
| Booking path | Choose an available date and time and proceed to the final review step. | The chosen slot remains visible on the review screen. |

### Limits of the examples

- These examples do not enable submissions.
- Preserve the shopper's actual inquiry choice.
- Do not describe a booking, form submission or purchase as performed when the check only reached the last step.

## Consent comparison

When requested, a consent focus can use:

- `intent`: Compare what the site requests and stores before any choice on the cookie banner, after Reject all, after Accept all with two pages browsed, after withdrawing in the same browser, and on a return visit.
- `successDescription`: Each of the five stages is recorded, or the report says which could not be established and why.
- `when`: The one-time or ongoing choice requested by the user.

### Limits of a consent focus

- This records browser behavior.
- It is not legal advice or a compliance certification.
- A saved focus is a requested area of attention; a later report establishes which steps were actually checked.
