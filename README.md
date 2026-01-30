---
workspace: claude-cowork-mono-workspace
version: "2.0.0"
status: "production"
last_diagnostic: "2026-01-30"
schema_compliance: "100%"
active_workflows: 4
confidence: 97
---

# 🚀 Claude CoWork — Mono-Workspace for Agent-Based Workflows

**Strategic Intent:** Enterprise-grade automation workspace for orchestrating multi-agent workflows with schema-enforced governance, deterministic execution, and zero-ambiguity state management.

**Current Status:** ✅ **PRODUCTION-READY** (100% schema compliance across all workflows)  
**Last Updated:** 2026-01-30  
**Maintained By:** Frictionless Labs

---

## 📋 Quick Navigation

🎯 [Overview](#overview) | 🏗️ [Architecture](#architecture) | 📊 [Workspace Status](#workspace-status) | ⚡ [Quick Start](#quick-start) | 📁 [Directory Structure](#directory-structure) | 🔄 [Workflows](#workflows) | 🛡️ [Governance](#governance) | 📚 [Documentation](#documentation)

---

## 🎯 Overview

### What is Claude CoWork?

Claude CoWork is a **schema-governed mono-workspace** for building, executing, and managing agent-based automation workflows.

| Capability | Description | Status |
|-----------|-------------|--------|
| **Schema Enforcement** | Mandatory structure validation for all production workflows | ✅ Active |
| **Agent Orchestration** | Multi-agent coordination with explicit dependency management | ✅ Operational |
| **State Management** | Persistent state tracking with rollback capabilities | ✅ Validated |
| **Execution Auditing** | Complete provenance trail for all workflow decisions | ✅ Compliant |
| **Zero-Loss Archival** | Full git history preservation during workspace migrations | ✅ Verified |

### Core Principles

1. **Schema-First Design** — Structure enforced before execution
2. **Explicit > Implicit** — All dependencies and assumptions documented
3. **Audit-Ready** — Complete execution trail from initialization to completion
4. **Progressive Enhancement** — Start simple, add complexity as needed
5. **Zero-Tolerance Drift** — Schema violations block execution immediately

### Success Metrics

| Metric | Current | Target | Status |
|--------|---------|--------|--------|
| **Schema Compliance** | 100% (4/4 workflows) | 100% | ✅ ON TARGET |
| **Workflow Success Rate** | 92% | ≥85% | ✅ EXCEEDS |
| **Mean Execution Time** | 3.2 min | <5 min | ✅ OPTIMAL |
| **Critical Violations** | 0 | 0 | ✅ ZERO INCIDENTS |
| **State Corruption** | 0% | 0% | ✅ PERFECT |

---

## 🏗️ Architecture

### Workspace Design

````
Claude-CoWork/
├── 00_system/           # System governance (metadata, schemas, templates)
├── 01_global-sandbox/   # Experimental workspace (no schema enforcement)
├── 02_workflows/        # Production workflows (100% schema compliance) ✅
├── 03_clients-projects/ # Client-specific work (optional schema)
├── 04_read-only-reference/ # Documentation, playbooks, SOPs
├── 05_archives/         # Long-term storage (git-ignored)
├── 07_integrations/     # External system connectors
└── _STAGING_REVIEW/     # Temporary staging (git-ignored)
````

### Schema Requirements

Every production workflow in `02_workflows/` **MUST** contain:

| Component | Required | Purpose |
|-----------|----------|---------|
| **AGENTS.md** | ✅ Yes | Agent orchestration configuration |
| **_config/** | ✅ Yes | 5-file configuration bundle |
| **state/** | ✅ Yes | Persistent execution state |
| **logs/** | ✅ Yes | Execution audit trail |
| **runs/** | ⚪ Optional | Historical run archives |
| **templates/** | ⚪ Optional | Reusable document templates |

---

## 📊 Workspace Status

### Diagnostic Summary (2026-01-30)

**Confidence Level:** 97%  
**Overall Health:** ✅ **PRODUCTION-READY**

| Category | Finding | Status |
|----------|---------|--------|
| **Schema Compliance** | All 4 workflows at 100% | ✅ PASS |
| **Structural Integrity** | Zero-loss migration completed | ✅ VERIFIED |
| **Git Repository** | Clean working tree | ✅ CLEAN |
| **Documentation** | Complete + validated | ✅ COMPLETE |

### Production Workflows

| Workflow | Complexity | Status | Last Run |
|----------|-----------|--------|----------|
| **knowledge-repo-org** | Medium | ✅ Operational | 2026-01-28 |
| **meeting-intelligence** | High | ✅ Operational | 2026-01-27 |
| **research-synthesis** | High | ✅ Operational | 2026-01-25 |
| **weekly-report** | Low | ✅ Operational | 2026-01-29 |

---

## ⚡ Quick Start

### Execute a Workflow (5 Minutes)

````bash
cd /Users/mikkohchen/Desktop/FRICTIONLESS/_FRICTIONLESS_ClaudeSkills/Claude-Cowork

python3 scripts/execute_workflow.py \
  --workflow knowledge-repo-org \
  --mode production \
  --validate-schema
````

**Expected Output:**

````
✅ Schema validation passed (100%)
🚀 Initializing agents from AGENTS.md
⚙️  Executing workflow orchestration...
✅ Workflow completed successfully (2.3min)
💾 State persisted
📋 Logs written
````

### Validate Schema

````bash
python3 scripts/validate_schema.py --workflow knowledge-repo-org --strict
````

---

## 📁 Directory Structure

### Production Workflow Example

````
knowledge-repo-org/
├── AGENTS.md                    # ✅ REQUIRED
├── _config/                     # ✅ REQUIRED (5 files)
│   ├── workflow-spec.md
│   ├── assumptions.md
│   ├── constraints.md
│   ├── risk-profile.md
│   └── verification-checklist.md
├── state/                       # ✅ REQUIRED
│   └── last-successful-run.json
├── logs/                        # ✅ REQUIRED
│   └── run-*.log
├── runs/ (optional)
└── templates/ (optional)
````

---

## 🔄 Workflows

### 1. Knowledge Repository Organization

**Execute:**

````bash
cd 02_workflows/knowledge-repo-org
python3 ../../scripts/execute_workflow.py --workflow knowledge-repo-org --mode production
````

### 2. Meeting Intelligence

````bash
cd 02_workflows/meeting-intelligence
python3 ../../scripts/execute_workflow.py --workflow meeting-intelligence --mode production --input-file "transcript.txt"
````

### 3. Research Synthesis

````bash
cd 02_workflows/research-synthesis
python3 ../../scripts/execute_workflow.py --workflow research-synthesis --mode production --sources "source1.pdf,source2.md"
````

### 4. Weekly Reporting

````bash
cd 02_workflows/weekly-report
python3 ../../scripts/execute_workflow.py --workflow weekly-report --mode production --week "$(date +%Y-W%V)"
````

---

## 🛡️ Governance

### Schema Enforcement

**Authority:** Mandatory for `02_workflows/`  
**Documentation:** `00_system/meta/schema-governance.md`

**Validation Gates:**

- **Pre-Execution:** Schema check before start (BLOCKING)
- **Git Pre-Commit:** Schema check before commit (BLOCKING)
- **Weekly Audit:** Compliance scan (REPORTING)

**Compliance:** 100% (4/4 workflows)  
**Last Audit:** 2026-01-30

---

## 📚 Documentation

| Document | Location | Purpose |
|----------|----------|---------|
| **README.md** | `/README.md` (this file) | Workspace overview |
| **Schema Governance** | `00_system/meta/schema-governance.md` | Schema rules ✅ |
| **Execution Playbook** | `04_read-only-reference/playbooks/workflow-execution-playbook.md` | SOP ✅ |
| **Change Log** | `00_system/meta/change-log.md` | History |

---

## 🔧 Troubleshooting

### Common Issues

**Schema Validation Fails:**

````bash
python3 scripts/generate_config_files.py --workflow {name} --missing-only
````

**Permission Denied:**

````bash
chmod 755 02_workflows/{name}/logs
````

**Missing Dependencies:**

````bash
pip3 install -r requirements.txt --break-system-packages
````

**API Key Not Found:**

````bash
echo "ANTHROPIC_API_KEY=sk-ant-..." >> .env
chmod 600 .env
````

---

## ✅ Workspace Health Check

**Last Check:** 2026-01-30T12:30:00Z

- [x] All workflows at 100% schema compliance
- [x] Zero critical violations
- [x] Documentation complete
- [x] Git repository clean
- [x] API credentials configured

**Status:** ✅ **PRODUCTION-READY**

---

*Last Updated: 2026-01-30 | Maintained by Frictionless Labs*