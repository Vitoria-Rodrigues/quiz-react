# Execution Plans Hub

This directory contains markdown-based execution plans and architectural migration roadmaps created by AI agents for multi-step tasks.

## Purpose

Plans in this directory break down large or complex refactors into sequential phases, verification gates, and atomic milestones. They track progress and decisions across long-running tasks.

## Guidelines

1. **Transient Artifacts**: Plan documents are operational tracking artifacts. Skills and plugins must remain decoupled and never contain required dependencies on specific plan files.
2. **Project Agnostic Patterns**: When designing new plans or templates, structure them with clear verification gates, rollback procedures, and environment-agnostic steps.
