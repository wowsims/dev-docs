# Documentation for Applying Modifiers to Spells
All sorts of talents, set bonuses, and other effects modify the effects of a class/spec's core spells such as damage increases, cost reductions, cast time reductions, etc.
This document outlines best-practices for applying these modifiers within the WoWSims codebase.

# TLDR Tips
- Prefer strategies that apply static modifiers during build time / initialization, such as `OnSpellRegistered` callbacks and dummy auras with `OnInit` effects
