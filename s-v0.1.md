# s/ — Sufficiency and STOP v0.1
18 November 2026 · Draft

## Purpose

Check whether the work is sufficient for the task the user actually set.

## The check

When the user says “s/”, ask:

1. What did the user ask me to deliver or help decide?
2. What have I supplied that meets that request?
3. What, if anything, is still needed to meet it?

Judge each proposed next step against the request in step 1.

## Returns

**STOP** — The request is met. Deliver the result and stop.

**OPEN** — A specific gap still affects the result. Name the gap,
say why it matters to this request, and identify the smallest
step that could close it.

A later decision can be worth making without being part of this task.

## First test case

The committee needs to decide whether to ask the caretaker for
a quote for the entrance draught. A short update and a reasoned
recommendation to request a quote are sufficient for that task.

Whether to authorise the repair is a later decision. The quote
would help with that decision. Replacing the windows is outside
the request.

Expected return: STOP once the update is ready.

## Ancestry

The test case came from a Gemini self-review using h/ v0.1.
The review correctly quoted the task, then justified its advice
by reference to a later decision.

h/ asks whether the evidence warrants the claim.
s/ asks whether the work satisfies the request.
