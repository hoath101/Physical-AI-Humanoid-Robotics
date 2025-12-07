# ADR-002: Middleware Selection for ROS 2 Integration in Humanoid Robotics Book

> **Scope**: Document decision clusters, not individual technology choices. Group related decisions that work together (e.g., "Frontend Stack" not separate ADRs for framework, styling, deployment).

- **Status:** Proposed
- **Date:** 2025-12-07
- **Feature:** 002-humanoid-robotics-book
- **Context:** ROS 2 uses DDS as its default middleware. The book needs to explain the choice of DDS and justify why it is preferred over alternative middleware options for robotic communication.

## Decision

The explicit rationale for using ROS 2's default DDS implementation is pending research.

## Consequences

### Positive

To be filled after research.

### Negative

To be filled after research.

## Alternatives Considered

- ZeroMQ
- Custom TCP/IP

## References

- Feature Spec: specs/002-humanoid-robotics-book/spec.md
- Implementation Plan: specs/002-humanoid-robotics-book/plan.md
- Related ADRs: N/A
- Evaluator Evidence: N/A
