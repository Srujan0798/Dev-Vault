# Jules - High-End Verification System

**Purpose**: Deep code verification after AI expansion of Dev Vault

---

## 🔄 WORKFLOW

```
1. EXPAND Dev Vault (using AI agents like Claude, Gemini)
         ↓
2. RUN Main Entry Point (scriptsDx/01_MAIN_ENTRY_POINT.py)
         ↓
3. RUN Jules Verification (this folder)
         ↓
4. COMMIT clean, verified files to GitHub
```

---

## 📁 Files in this folder

| File | Purpose |
|------|---------|
| `check_corruption.py` | Deep encoding/corruption check using chardet |
| `fix_corruption.py` | Auto-fix mojibake and encoding issues using ftfy |
| `generate_manifest.py` | Generate checksums and manifest for all files |
| `AGENTS_GUIDE.md` | Guide for AI agents maintaining Dev Vault |
| `vault_health.json` | Last health check results |
| `vault_manifest.json` | File checksums and metadata |

---

## 🚀 Usage

### Check for corruption

```bash
python scriptsDx/jules/check_corruption.py
```

### Fix encoding issues

```bash
python scriptsDx/jules/fix_corruption.py
```

### Generate manifest

```bash
python scriptsDx/jules/generate_manifest.py
```

---

## 📋 When to Use

Use Jules tools **AFTER**:

- Adding new content to Dev Vault from AI agents
- Importing data from external sources
- Major expansions or refactoring

Jules provides **deeper verification** than the main entry point scripts.

---

## 🔗 Integration with Main System

The main entry point (`01_MAIN_ENTRY_POINT.py`) handles:

- 53 scripts × 45 files = 2,385 operations
- Regular validation and fixing

Jules handles:

- Deep encoding verification
- Corruption detection with chardet
- Manifest generation for tracking
