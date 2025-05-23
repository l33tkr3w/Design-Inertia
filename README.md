# Design Inertia: Why We Keep Writing Code for Problems That Language Could Solve

*By Cory Hafer*  
*May 2025*

## TL;DR

Developers often rely on code-heavy solutions for problems that could be handled more flexibly through language-based logic. This tendency stems from inherited design habits rooted in pre-language-system paradigms. I call this "Design Inertia": a pattern of solving new problems with old tools.

## The Core Idea

Modern systems can interpret natural language and carry out high-level reasoning. Despite this, many of us continue to build workflows the way we always have: by writing explicit, procedural code.

For example, instead of describing what we want in plain terms:

"If a task contains the word 'urgent', send it to X. If it mentions 'schedule', send it to Y. Otherwise, archive it."

We write:

```python
def route_task(task):
    if "urgent" in task:
        return "fast_action"
    elif "schedule" in task:
        return "calendar"
    else:
        return "archive"
```

This works, but it is rigid. It lacks the flexibility of language and doesn't adapt well to varied input or nuance. Most importantly, it ignores the strengths of systems that understand language natively.

## Why This Happens

The reason is simple. Most developers were trained on traditional programming methods. The ecosystems, examples, and documentation that shaped us are all built around explicit logic. So when we approach new systems, we fall back on what we know.

For decades, code was the only way to encode logic. Every flowchart, class hierarchy, and state machine had to be spelled out in full detail. Even now, many developers write as if the system cannot reason unless they micromanage every step.

But that assumption is no longer true. Systems today can interpret intent, follow instructions, and adapt to soft rules, all without being wrapped in procedural control flows.

## This Is Design Inertia

Design Inertia is what happens when a platform evolves but our habits do not.

We've seen this before. Early websites were laid out like newspapers. Early smartphones mimicked desktop UIs. People printed emails out of habit.

And now we are seeing it again. We build modern systems that understand language, then trap them in rigid code as if they were dumb interpreters.

It is not about rejecting code. It is about recognizing when code is no longer the best way to express a solution.

## What This Looks Like

If you're building a tool with semantic reasoning or agentic capabilities, here's what Design Inertia might look like:

Writing long if-else chains instead of expressing intent in plain instructions

Creating unnecessary wrappers around simple behavior

Managing low-level state transitions manually instead of reasoning through goals

Trying to hardcode logic that a natural language query could handle more efficiently

In these cases, we end up writing more code than needed, making the system less adaptable, and losing out on the reasoning capabilities we already have.

## A Better Way Forward

**Design in Language First**
Write down what you want the system to do in plain language. Build logic as instructions. Then decide if any of it needs to be turned into code for precision or performance.

**Use Instructions as Interfaces**
Build workflows using readable instructions passed between modules or components. Not everything has to be a function call or a method. Language can be a powerful interface.

**Avoid Premature Abstraction**
Don't start with architecture. Start with intent. Let the problem shape the structure, not the other way around.

**Let the System Interpret**
If you've built or are using a system that understands language, let it. Don't smother it with hardcoded scaffolding.

## The Future of Building

We're entering a new era of design, one where conversation, intent, and soft logic will take precedence over rigid structures and code-heavy pipelines.

Every transition feels awkward. The first instinct is to drag old methods into the new world. But if we keep doing that, we'll miss the opportunity to build something better.

Code was a means, not an end. It was the best tool we had. Now we have something that, in some contexts, can do more with less. And we should build like we believe that.

## Let's Talk

Design Inertia is something we all experience, even if we don't have a name for it. If this concept resonates with you, share it. Build with it. Spot it in the wild. Talk about it.

And maybe next time, before writing the function, just say what you want.
