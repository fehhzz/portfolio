# SKY-OS — Portable Knowledge & Agent Context

[← Portfolio](README.md)

## Problem

Maintain reliable project context across sessions and environments without relying entirely on conversation history.

## Implementation

A private Markdown knowledge system organizes company context, workstream checkpoints, territorial routing, reusable agent instructions and authorization boundaries. PowerShell utilities and reports support validation of the document structure.

**Stack:** Markdown, Git, agent Skills and PowerShell.

## Technical decisions

- A current-state document establishes the authoritative checkpoint.
- Agent routing directs reading toward the relevant workstream instead of loading all context.
- Status, scope and approval boundaries are documented explicitly.
- Knowledge and operational instructions are kept distinct from client records and private session material.

## Stage

The portable MVP is recorded as merged into the private main branch. The first real notebook cold-start test remains pending. This public case describes the knowledge architecture and does not publish internal company strategy or activate operational workflows.

## Em português

Sistema de conhecimento para continuidade de projetos, contexto de agentes e organização operacional. Demonstra documentação estruturada, controle de estado e portabilidade de contexto entre ambientes.
