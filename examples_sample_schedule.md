# Sample Human-Readable Output

## Kanban
### To-Do
- T-003 | UI: Login page | Riya | M | size 3 | due 2025-09-05
- T-004 | Infrastructure: S3 bucket | Yash | M | size 2 | no due
- T-006 | Docs: README | Yash | L | size 1 | no due

### In-Progress
- T-002 | Auth API endpoint | Sam | H | size 5 | due 2025-09-06
- T-005 | Bug: 500 on /tasks | Sam | H | size 2 | due 2025-09-02

### Done
- T-001 | Setup repo & CI | Yash | H | size 2 | due 2025-09-03

---

## Sprint Plan (2025-09-01)
**Sam**
- 10:00–12:00 → T-005 (Reproduce bug)
- 13:00–15:00 → T-002 (Auth routes)

**Yash**
- 10:00–12:00 → T-004 (S3 bucket setup)

---

## Risks & Mitigations
- **Risk:** T-005 deadline very near.  
  **Mitigation:** Pair programming or prioritize over new features.
- **Risk:** Sam at capacity.  
  **Mitigation:** Temporarily reassign T-004 to Riya after UI block.

## Next 5 Actions
1. Close T-005 before noon tomorrow.  
2. Add tests to T-002.  
3. Create buckets/policies for T-004.  
4. Start T-003 once API stable.  
5. Draft docs (T-006) during downtime.
