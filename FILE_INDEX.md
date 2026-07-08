# Email Extraction Project - File Index

## Overview
Complete email extraction dataset for 608 domains with support/business emails only.

---

## Primary Data Files

### 1. comprehensive_email_list.json (87 KB)
**Format:** JSON  
**Records:** 316 domains with support emails  
**Purpose:** Complete dataset with all metadata

**Structure:**
```json
{
  "domain": "example.com",
  "contact_emails": ["support@example.com", "info@example.com"],
  "email_count": 2,
  "security_program": "responsible_disclosure",
  "security_contact": "security@example.com",
  "security_platform": "NOT STATED",
  "security_rewards": "NOT STATED"
}
```

**Fields:**
- `domain`: Company domain name
- `contact_emails`: Array of support/business email addresses
- `email_count`: Number of support emails for this domain
- `security_program`: Type of security program (if any)
- `security_contact`: Security contact email (if available)
- `security_platform`: Security platform used (HackerOne, etc.)
- `security_rewards`: Reward information (if available)

---

### 2. comprehensive_email_list.csv (26 KB)
**Format:** CSV (pipe-delimited)  
**Records:** 316 domains with support emails  
**Purpose:** Spreadsheet-compatible format

**Columns:**
```
Domain | Contact Emails | Email Count | Security Program | Security Contact | Security Platform | Security Rewards
```

**Example:**
```
example.com | support@example.com|info@example.com | 2 | responsible_disclosure | security@example.com | NOT STATED | NOT STATED
```

---

### 3. all_emails_flat.txt (9.1 KB)
**Format:** Plain text (one email per line)  
**Records:** 465 support email addresses  
**Purpose:** Bulk email export, mailing lists

**Format:**
```
support@example.com
info@example.com
sales@example.com
...
```

---

## Reference Files

### 4. domain_email_mapping.json (85 KB)
**Format:** JSON  
**Purpose:** Quick domain-to-email lookups

**Structure:**
```json
{
  "example.com": ["support@example.com", "info@example.com"],
  "another.com": ["contact@another.com"],
  ...
}
```

---

### 5. master_security_extraction.json (215 KB)
**Format:** JSON  
**Records:** 608 domains (all)  
**Purpose:** Complete security program data

**Structure:**
```json
{
  "domain": "example.com",
  "security_program": "responsible_disclosure",
  "security_contact": "security@example.com",
  "security_platform": "NOT STATED",
  "security_rewards": "NOT STATED"
}
```

---

### 6. security_programs_all_domains.csv (81 KB)
**Format:** CSV  
**Records:** 608 domains (all)  
**Purpose:** Security program analysis

**Columns:**
```
Domain | Security Program | Security Contact | Security Platform | Security Rewards
```

---

## Documentation Files

### 7. README.txt
**Purpose:** Project overview and quick start guide  
**Contents:**
- Project description
- File descriptions
- Data structure
- Usage examples
- Quality metrics

---

### 8. FINAL_SUMMARY.txt
**Purpose:** Project statistics and completion status  
**Contents:**
- Extraction statistics
- Security programs identified
- Top domains by email count
- Filtering applied
- Quality metrics
- Project completion info

---

### 9. FILE_INDEX.md (this file)
**Purpose:** Detailed file format documentation  
**Contents:**
- File descriptions
- Data structures
- Field definitions
- Usage guidelines

---

### 10. DELIVERY_CHECKLIST.txt
**Purpose:** Project completion checklist  
**Contents:**
- All tasks completed
- Quality assurance checks
- Deliverables verified

---

## Data Statistics

| Metric | Value |
|--------|-------|
| Total Domains | 608 |
| Domains in Master | 590 |
| Domains with Support Emails | 316 (53.6%) |
| Total Support Emails | 465 |
| Unique Email Addresses | 465 |
| Security Programs Found | 16 |

---

## Email Categories Included

✓ Support: support@, help@, contact@, info@  
✓ Sales: sales@, hello@, business@, inquiry@  
✓ Media: press@, media@, partnerships@, partners@  
✓ HR: careers@, jobs@, hr@, recruitment@  
✓ Finance: billing@, payments@, finance@, accounts@  
✓ Operations: admin@, team@, connect@, reach@  
✓ Feedback: feedback@, service@, customer@, care@  
✓ Success: success@, onboarding@, security@, privacy@  
✓ Legal: legal@, compliance@, dpo@  

---

## Filtering Applied

**Removed:**
- Personal emails (firstname@domain, name.surname@domain)
- Generic personal patterns (name123@domain)
- Domains with no support emails (274 domains)

**Kept:**
- All support/business email patterns
- All security-related emails
- All company contact emails

---

## Usage Guidelines

### For Email Marketing
Use `all_emails_flat.txt` for bulk email operations

### For Data Analysis
Use `comprehensive_email_list.csv` in Excel/Google Sheets

### For Programmatic Access
Use `comprehensive_email_list.json` in your application

### For Security Analysis
Use `security_programs_all_domains.csv` for security research

### For Quick Lookups
Use `domain_email_mapping.json` for domain-to-email mapping

---

## Quality Assurance

✓ All 608 domains processed  
✓ 590 domains in master dataset  
✓ 316 domains with support emails  
✓ 465 support emails extracted  
✓ All personal emails removed  
✓ All data validated and deduplicated  

---

## Project Information

**Status:** ✓ COMPLETE  
**Last Updated:** July 8, 2026  
**GitHub:** https://github.com/nikhilkaushik12345/email-extraction-608-domains  

---
