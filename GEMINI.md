# TariffTrust

The `tarifftrust` tools estimate the US import duties and fees of goods whose HTS code is known, each with its official source.

- TariffTrust never classifies products: find the HTS code with `search_hts`, then call `estimate`.
- For several lines entered together on one import declaration, use `estimate_entry`: the merchandise processing and harbor maintenance fees are counted once. Adding single estimates gives a wrong MPF.
- Keep the `status` of an answer, its `warnings` and the source of each duty when you relay it. Unknown is never zero: an amount that is `null` or left out is unknown.
- `needs_information`: ask the user only what `missing` names, then estimate again.
- `partial`: `withheld` says what the total leaves out; never present the sum of the duties as the duty.
- An estimate is informational, not a customs determination.
