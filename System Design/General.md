### Single Source of Truth
Single Source of Truth (SSOT) is a design principle stating that a particular piece of data or state should be owned and maintained in exactly one place, and every other part of the system reads from (but doesn’t independently update) that single “authoritative” source.

Why it matters
Consistency: With only one place to update, you avoid having out-of-sync copies floating around.

Maintainability: Bugs related to stale or divergent data are dramatically reduced.

Clarity: It’s clear where the “real” value lives—teams know exactly where to look when they need to change something.


### Canonical:

In this context, “canonical” simply means the authoritative, standard, or “official” version of something—the one true source that everyone else refers to.

Etymology: Comes from the notion of a “canon,” i.e. a set of rules or works that are officially recognized.

In data/software: A canonical data store is where the “correct” values live; everything else reads from (and, ideally, writes through) that single place.

In URLs (web SEO): A canonical URL is the “preferred” address for a page when the same content is reachable via multiple links—you signal to search engines which one is the official version.

In file systems: A canonical path is the fully-resolved absolute path (no symlinks, . or ..), used to avoid ambiguity.

So when we said “identify your canonical store,” we meant: pick the one location that you treat as the definitive source of your data or configuration—no competing copies allowed.
